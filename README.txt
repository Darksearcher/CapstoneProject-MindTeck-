Instructions for using/ running my web application.

 1. There are two databases used in this system
 1.1. Users
 a) Should work out of the box while using my application
 1.2. The model for the web application
 a) I believe you need to create this one as it doesn't come attached, I'm not sure how to change this or how to include the databse
 b) My only solution is to provide the queries for filling the databases and asking the assessor to run WebDatabase.edmx.sql, or generating the database from the model.

Query for carts

SET IDENTITY_INSERT [WebDatabase].[Carts] ON
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (3, 1, 3, 27)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (9, 43, 4, 27)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (11, 2, 5, 28)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (12, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (13, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (14, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (15, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (16, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (17, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (18, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (20, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (21, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (22, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (24, 3, 4, 38)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (25, 1, 5, 38)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (26, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (27, 0, NULL, NULL)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (31, 3, 6, 27)
INSERT INTO [WebDatabase].[Carts] ([Cart_ID], [Quantity], [Product_ID], [WebUserID]) VALUES (32, 3, 9, 27)
SET IDENTITY_INSERT [WebDatabase].[Carts] OFF




Query for Order Histories

SET IDENTITY_INSERT [WebDatabase].[OrderHistories] ON
INSERT INTO [WebDatabase].[OrderHistories] ([OrderHistory_ID], [WebUsersId], [OrderDate]) VALUES (1, 38, N'2014-09-28 17:28:48')
INSERT INTO [WebDatabase].[OrderHistories] ([OrderHistory_ID], [WebUsersId], [OrderDate]) VALUES (2, 38, N'2014-09-28 19:25:37')
SET IDENTITY_INSERT [WebDatabase].[OrderHistories] OFF


Query for Products

SET IDENTITY_INSERT [WebDatabase].[Products] ON
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (3, N'Tide', N'Tides reinventing the way you do laundry! New Tide Pods is a multi-dimensional laundry detergent that cleans, fights stains, and brightens in one. No more pouring. No more lugging. No more spills. Just toss one in—it''s that easy!', 13, 19.99, N'Tide', N'http://www.mydiscountcoupon.com/blog/wp-content/uploads/2014/08/Tide-logo.jpg')
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (4, N'Mass Effect 3', N'Battle as Commander Shepard on many worlds across the galaxy as you unite the ultimate force to take back the Earth before it''s too late', 43, 39.99, N'Bioware', N'http://ecx.images-amazon.com/images/I/71%2BGnpj0OML._SL1007_.jpg')
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (5, N'LG Nexus 5', N'At only 4.59 oz and 8.59 mm thin, it''s the most powerful Nexus phone yet. Speed and power to spare. With 4G/LTE and ultra-fast Wi-Fi, Nexus 5 keeps you connected at blazing speeds. Add in the cutting-edge 2.26GHz Qualcomm SnapdragonTM 800 processor and you''ll race through games, zip around the web and switch between apps at the flick of a finger. Stunning 5 display. More room to do what you do, and better colors too.', 10, 599.99, N'Google', N'http://ecx.images-amazon.com/images/I/41dy1h6PB2L.jpg')
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (6, N'GTX 980', N'The new EVGA GeForce GTX 980 is powered by the next-generation NVIDIA Maxwell architecture, giving you incredible performance, unmatched power efficiency, and cutting-edge features.', 3, 689, N'EVGA', N'http://ecx.images-amazon.com/images/I/71Tagdynd9L._SL1500_.jpg')
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (7, N'Super Smash Bros. - Nintendo 3DS', N'New characters items and arenas add a freshly reinvigorated look and feel. Amiibo will add a different dimension to game play as classic Nintendo characters interact wirelessly in the game.', 0, 39.99, N'Nintendo', N'http://ecx.images-amazon.com/images/I/61KVPjyuLXL.jpg')
INSERT INTO [WebDatabase].[Products] ([Product_ID], [Name], [Description], [Stock], [Price], [Company], [PictureURL]) VALUES (9, N'Playstation', N'Game Console for all ages!', 3, 1.99, N'Test', N'http://gadgets-ntech.com/wp-content/uploads/2013/12/ps5.jpg')
SET IDENTITY_INSERT [WebDatabase].[Products] OFF

Query for Webusers

SET IDENTITY_INSERT [WebDatabase].[WebUsers] ON
INSERT INTO [WebDatabase].[WebUsers] ([Id], [Administrator], [FirstName], [LastName], [Address], [Email], [Number], [Anonymous], [CartId]) VALUES (27, 0, N'Anonymous', N'User', NULL, NULL, NULL, 1, 3)
INSERT INTO [WebDatabase].[WebUsers] ([Id], [Administrator], [FirstName], [LastName], [Address], [Email], [Number], [Anonymous], [CartId]) VALUES (30, 0, N' ', N' ', N' ', N'vic9050@hotmail.com', 1211231234, 0, 12)
INSERT INTO [WebDatabase].[WebUsers] ([Id], [Administrator], [FirstName], [LastName], [Address], [Email], [Number], [Anonymous], [CartId]) VALUES (38, 0, N'Victor', N'Viglianti', N'241 Brentwood Avenue', N'zxcv@vcxz.com', 1111111111, 0, 21)
INSERT INTO [WebDatabase].[WebUsers] ([Id], [Administrator], [FirstName], [LastName], [Address], [Email], [Number], [Anonymous], [CartId]) VALUES (39, 0, N' ', N' ', N' ', N'asdf@fdas.ca', 1211231234, 0, 22)
INSERT INTO [WebDatabase].[WebUsers] ([Id], [Administrator], [FirstName], [LastName], [Address], [Email], [Number], [Anonymous], [CartId]) VALUES (60, 1, N'Admin', N'Admin', N'', N'admin@admin.com', 1211231234, 0, 27)
SET IDENTITY_INSERT [WebDatabase].[WebUsers] OFF


 
 1. I have provided the following test user cases
 1.1.  Login as an administrator
 a) admin@admin.com 
 b) Password: Admin1!
 1.2. Login as test user 
 a) zxcv@vcxz.com
 b) Passowrd: Zxcv1!
 1.3. Login as anonymous
 a) Make sure to be logged out!!

This worked perfectly on my machine running Windows 7, the latest version of Google Chrome, and visual studio 2013.  If there are any issues with this project please do not hesitate and reach me at vic9050@gmail.com.
