# CryptoWallet
CREATE TABLE [Crypta](
	[ID] varchar(255) not null,
	[Name] varchar(255) not null,
	[Price] float not null,
	[Count] float not null
)
CREATE TABLE [User](
	[ID] varchar(255) not null,
	[NickName] varchar(255) not null,
	[CreatedOn] datetime,
	[UpdateOn] datetime,
	[IsDelete] bit
)
CREATE TABLE [Wallet](
	[ID] varchar(255) not null,	
	[UserID] varchar(255) not null,
	[CryptID] varchar(255) not null,
	[CreatedOn] datetime,
	[UpdateOn] datetime,
	[IsDelete] bit
)
CREATE TABLE [Transfer](
	[ID] varchar(255) not null,
	[FirstUserID] varchar(255) not null,
	[SecondUserID] varchar(255) not null,
	[CryptID] varchar(255) not null,
	[CreatedOn] datetime,
	[IsDelete] bit
)
INSERT INTO [User] VALUES('001','Serii')
INSERT INTO [User] VALUES('002','Mash2_2')
INSERT INTO [User] VALUES('003','Uwe2oo')
INSERT INTO [User] VALUES('004','O_Owl')

INSERT INTO [Crypta] VALUES('723','BTC',41546.80,0.00001)
INSERT INTO [Crypta] VALUES('719','ETH',3019.71,0.004)
INSERT INTO [Crypta] VALUES('002','BTC',41546.80,0.01)
INSERT INTO [Crypta] VALUES('982','DOGE',0.15,200)
INSERT INTO [Crypta] VALUES('823','ETH',3019.71,2.2)
INSERT INTO [Crypta] VALUES('125','BNB',424.08,8.8)
INSERT INTO [Crypta] VALUES('923','BTC',41546.80,0.8)

INSERT INTO [Wallet] VALUES('823','001','723')
INSERT INTO [Wallet] VALUES('823','001','719')
INSERT INTO [Wallet] VALUES('017','002','002')
INSERT INTO [Wallet] VALUES('253','003','982')
INSERT INTO [Wallet] VALUES('824','004','823')
INSERT INTO [Wallet] VALUES('825','004','125')
INSERT INTO [Wallet] VALUES('825','004','923')
