Documentation
=============

1).  Introduction

1.1) Project Profile
		
		
	
Project Title	Virtual Live Stock Management  System
Type	 Mobile Application
Tools used	Dreamweaver, ADT (Android Development Tool), MySql
Frontend	Android Java, Android, PHP
Backend	SQLite, MySql
Other tools	Edraw 6.3, MS Office 2007

		
	




2) Environment Description

2.1) Hardware and Software Requirements



	Hardware Requirements
	Smart mobile device
	128 mb of RAM
	10 mb internal storage

	Software Requirements
	Android OS  version 2.2 or higher
	Internet connectivity





3) Existing System

3.1) System components
3.2) Drawbacks of existing systems

 

3.1) System components

The development of the Virtual Live Stock Management System requires the facility that introduces the concept of centralized database and decentralized client side applications so that system can be updated any time with live environment and thus client is able to have services of getting Market information at any point of time.
These must  be combined in such a way that new information can be updated as quick as possible and therefore centralized database concept becomes very much useful.
There  are several system components that combines and makes up a broadly useful “Virtual Live Stock Management System”
	Virtual Live Stock Management Information
	Market Information
	Inventory Information
	News updates
	Important Notifications
	Coupons that enables having information of any particular Product
	Automatic updates of Markets
 

3.2) Drawbacks of existing systems

	Existing system doesn’t encompass all features in single system.
	Existing systems doesn’t provides automatic update feature.
	Existing system implements static data structure.
	User have to pay money for using application.

 
4) System Planning

4.1) Requirement analysis and data gathering


	Facilities to create centralize admin application and de-centralize client application communication architecture.
	Facility to create simple and fully loaded mobile application for entertainment.
	Facility to create a new user account
	Facility to save offline data to enable application to work offline
	Facility to view top user’s profile.
	Facility to get news updates of admin.
	Facility to track user’s position and get the transactions details.
	Facility to provide price logs of the items from very start of item availability.
	Give admin full control of market and also the atomization of logging.
	Application should automatically check for new updates at server, like while booting, starting application, connecting to internet.

 
5) Proposed System

5.1) Scope
5.2) Objectives
5.3) Constrains 
5.4) Expected advantages

 
5.1) Scope

“Virtual Live Stock Management System” encompasses two entities User & Admin both of them having different scope in system and is described here.

Ω	User 

o	Can create own account for authentication
o	Can Buy and sell items for gain virtual profit.
o	Can view his/her inventory
o	Can view his/her previous transaction
o	Can compare his records with top players.
o	Can also get news and notification.

Ω	Admin

o	Can add items.
o	Can delete items.
o	Can Update Items.
o	Can add news.
o	Can add coupons.
o	Can manage users.


 

5.2) Objectives

	The purpose of this project is to develop mobile applications using an SDK so that it leads to consistent & rapid development approach. And also it should leads to less maintenance cost of an application.

	The main objective of the system is pure entertainment with learning.


	The user can buy and sell in miniature market scenario for little essence of competition.

	The system build in client server architecture based multiple client enable system so each user is connected with centralize system for administration purpose.


	The system is the product of the company so it is use for marketing purpose.

.

Feature includes:
	virtual livestock management system is the real time miniature game based upon essence of stock market system
	The user of the application uses it for entertainment as well as learning the way of stock market.
	User can compete with other user by top chart list.
	The game is used ad client server communication architecture so the control is centralized by admin.
	the virtual livestock system is useful for marketing also, it comes with news functionality.
	The system is a product of over company which will be distributed over the world and leave a mark on users.
 

5.3) Constraints 

	Android device must for this application for any other platform it will be useless.
	Internet access must for stay updated with server.
	While using Market or loading news images if internet disconnects it could fail operation
	High processing speed recommended for smooth animations
 

5.4) Expected advantages

	Stay updated with market.
	Should provide detailed information about particular User products Detail.
	Should provide current news update.
	Should include the feature of automatically update of system.
	 Should give important notifications.
	Should provide  Products & Coupons information.
	Should provide better performance.
	Should enable users to customize their personal settings.
	Should have very impressive user interface.
	Should allow users to customize their application interface.




 
6) Detail Planning

6.1 Use case Diagram
	6.2 Activity Diagram
	6.3 Sequence Diagram
6.4 Data Dictionary

 
	

6.1) Use Case Diagram
A use case diagram in the Unified Modelling Language (UML) is a type of behavioural diagram defined by and created from a Use-case analysis. Its purpose is to present a graphical overview of the functionality provided by a system in terms of actors, their goals (represented as use cases), and any dependencies between those use cases.


 


 





 





6.2 Activity Diagram
 
 
 


 


 


6.3 Sequence Diagram 
 




  





 
 
6.4  Data Dictionary           

Name	tbl_login
Alias	None
Where used / How used	To store User login information
Input:- Login info to verify
Output:- Verified login info
Content description	User_Id + User_name +user_ Password + user_email +  user_image+ user_date_time + user_account
Supplementary Information	User_id must be unique and AutoIncrement all other fields may not be unique.


Name	tbl_item
Alias	None
Where used / How used	To store product Virtual Live Stock Management System.
Input:- Item
Output:- requested product
Content description	Item_Id + Item_name + Item_price + Item_description+ entered_date_time
Supplementary Information	Item_Id must be unique and AutoIncrement and all other fields may not be unique.



Name	tbl_news
Alias	None
Where used / How used	To store News information.
Input:- News info
Output:- requested news info date wise
Content description	News_Id + News_Date + News_Description  +News_image
Supplementary Information	News_Id must be unique and not null annd AutoIcrement, it is used to identify each news uniquely,
While other fields doesn’t need to be unique.










Name	tbl_inventory
Alias	None
Where used / How used	To store product information.
Input:-  Inventory qantity info
Output:- requested qantity info

Content description	Inventory_Id + User_Id + Item_id + inventory_qty 

Supplementary Information	Inventory_Id must be unique and not null and AutoIncrement while all other may not be unique, Item_Id must be one of from table tbl_item.

 



Name	tbl_coupon
Alias	None
Where used / How used	To store coupon info
Input:- coupon info
Output:- requested coupon discount info
Content description	Coupon_id + Coupon_title + Coupon_code + Coupon_description + Coupon_discount_amount + Coupon_percentage + Coupon_startdate + Coupon_enddate
Supplementary Information	Coupon_id must be unique and not null and AutoIncrement while all other may not be unique and all are required.














Name	tbl_transaction
Alias	None
Where used / How used	To store Transaction info from users
Input:- Transaction info
Output:- requested Transaction info
Content description	transaction _id + user_id + item_id + transaction _qty + transaction_unit_price + transaction_date_time+ transaction _type
Supplementary Information	transaction _id must be unique and not null and AutoIncrement while all other may not be unique but all are required.



7).	System Design

7.1) Database Design
7.2) Input Design
7.3) Output Design
 
7.1) Database Design

tbl_login
*(MySql)
Field	Data type	Null	Constraints
User_id	INT(11)	NOT NULL	AUTOINCREMENT
User_name	VARCHAR(45)	NOT NULL	Username for login
User_password	VARCHAR(45)	NOT NULL	Password for login
User_email	VARCHAR(45)	NOT NULL	Email id for login
User_image	Text	NOT NULL	Image for profile
User_date_time	DATETIME	NOT NULL	login date time
User_account	INT	NOT NULL	User points by Default

PRIMARY KEY (user_id)

tbl_news
*(MySql & SQLite)
Field	Data type	Null	Constraints
news_id	INT(11) 	NOT NULL	AUTOINCREMENT
news_date	DATE	NOT NULL	Timestamp for when news inserted
news_description	TEXT	NOT NULL	Description of news
news_image	TEXT	NOT NULL	News Image

PRIMARY KEY (news_id)

tbl_coupon
*(MySql & SQLite)
Field	Data type	Null	Constraints
Coupon_id	INT(11) 	NOT NULL	AUTOINCREMENT
Coupon_title	VARCHER(100)	NOT NULL	Title of Coupon
Coupon_code	VARCHER(10)	NOT NULL	Coupon Code
coupon_description	TEXT	NOT NULL	Coupon Description
coupon_discount_amount	INT(11)	NOT NULL	Coupon Discount
coupon_percentage	INT(3)	NOT NULL	Percentage 
coupon_startdate	DATETIME	NOT NULL	Timestamp for  Coupon started
coupon_enddate	DATETIME	NOT NULL	Timestamp for  Coupon Ended

PRIMARY KEY (coupon_id)
	
tbl_discount
*(MySql & SQLite)
Field	Data type	Null	Constraints
Discount_id	INT(11) 	NOT NULL	AUTOINCREMENT
User_id	INT(11)	NOT NULL	Description of  user id
Coupon_id	INT(11)	NOT NULL	Description of  coupon  id

PRIMARY KEY (discount_id)



tbl_inventory
*(MySql & SQLite)
Field	Data type	Null	Constraints
inventory _id	INT(11) 	NOT NULL	AUTOINCREMENT
User_id	INT(11)	NOT NULL	Description of  user id
Item_id	INT(11)	NOT NULL	Description of item id
Inventory_qut	INT(11)	NOT NULL	User Inventory quantity

PRIMARY KEY (inventory_id)


tbl_item
*(MySql)
Field	Data type	Null	Constraints
item _id	INT(11)	NOT NULL	AUTOINCREMENT
item _name	VARCHAR(100)	NOT NULL	Product  Name
item _price	INT(11)	NOT NULL	Item Price
item_image	TEXT	NOT NULL	Item Image
item _desription	TEXT	NOT NULL	Description Image
entered_date_time	DATETIME	NOT NULL	Timestamp for  item Entered

PRIMARY KEY (item_id)



tbl_price_log
*(MySql & SQLite)
Field	Data type	Null	Constraints
price_log_id	INT(11) 	NOT NULL	AUTOINCREMENT
item_id	INT(11)	NOT NULL	Description of item id
Price	INT(11)	NOT NULL	 Price item
price_log_date_time	DATETIME	NOT NULL	Timestamp for when Price inserted

PRIMARY KEY (price_log _id)

tbl_transaction
*(MySql & SQLite)
Field	Data type	Null	Constraints
transaction _id	INT(11) 	NOT NULL	AUTOINCREMENT
uesr_id	INT(11)	NOT NULL	Description of user id
item_id	INT(11)	NOT NULL	Description of item id
transaction_qty	INT(11)	NOT NULL	Description of  Transaction qty
transaction_unit_price	INT(11)	NOT NULL	Transaction Price
transaction _date_item	DATETIME	NOT NULL	Timestamp for when Transaction done
transaction _type	INT(11)	NOT NULL	Transaction is buy or sell

PRIMARY KEY (coupon_id)
 

7.2) Input Design & Output Design



Login.php
	Admin using this page to login to system. 


	

AddItems.php
		Using this page admin can add Item Into the System.

 



	

item.php
	View of Items.
	Admin can edit and delete using action for edit & delete icons.
 
 




AddNews.php
	Admin uses this page to add news information to database.
	Admin also uses this interface for updating news information.




 


 



News.php
	Admin uses this page to view current news data.
	Admin can perform edit and delete operations using action buttons.

 






AddCoupons.php
	Admin uses this page to add Coupons  information and Discounts.
	
 



 


Coupon.php
	Admin uses this page to view current mantra information.
	Admin can delete mantra by using delete action button.
 
 


 


User.php
	Admin uses this page to view User details .
	Admin cannot Change  Any information  from here.

 





Inventory.php
	Admin can  View Inventory information using this page .

 
Device Home::


  			 s

 
Application Icon
		This is an application  icon. We can access an application by clicking on this icon.

	


Splash Page :
	
	



.





Splash page :
	This will Check The Internet Connection of Application if it is connected then enter else give Error of Network established Failed.
		 
Splash Page :

		 

Login Activity
 User can Login or SignUp and also know about   the company using this activity.
 

Sign In :

		 

Login Activity
 		User can Login .User can login by typing an id and password. 



Sign Up :

		 

Sign Up Activity
 User can Login or SignUp and also .New user can signup here by filling details.


Application Home Page :

		  

Main Activity
Main Menu Activity of application. 
Using this list user can navigate to various other activities

Market:
			
		 

Market Activity 
Displays current Market updates. 


Bye Item :	

		 

Buy Activity 
This represents an different types of items. user \can  buy items here.

     Transaction:
		 

Transaction  Activity 
Displays user transaction related buy and selling items. 
 
InventoryItem :

  
Inventory Activity
This represents an inventory about an user who login. User can see his detailed inventory. And also can sell his items from here. 

 
Sell Item :
		
		 

Sell Activity
		This represents an different types of items. user \can  sell items here.


News :	

	 

News  Activity 
Displays for news related by market .  


Top Charts :
	
		 
Top charts Activity 
Displays information highest scores done by user. 

Coupons:

		 
Coupons Activity 
Displays different types for coupons. That represent discounts offers.  

Setting :

		 
Setting Activity 
          User can edit profile, can view notification,can see contact us,and can logout from here

Edit Prpfile:

		 
Edit Activity 
User can edit our profile. 
		




8).	Software Testing

The testing Process focuses on the logical interrelations of the software ensuring that all statements have been tested and on the functional externals that is, conducting test to uncover errors and ensure that defined input will produce actual results that agree with required results.   
There are following types of testing which we have done in our system.

•	Unit Testing
•	Integration Testing
•	System Testing
•	Acceptance Testing
•	Regression Testing

•	UNIT TESTING
•	System is first tested using unit testing.
•	Unit testing is test of code written by a single programmer.
•	In Unit testing each programmer’s, each module is tested which is isolation from the rest of system.

No.	Input	Condition checked	Expected Output
1	NULL	No Entry From User	Err Msg
2	C102637654602	Alpha-Numeric for Phone No.	Err Msg
3	9102637654602	Phone No Length Check	Validated No
4	12345678912	Check more then 10 Digit for Mobile No	Err Msg
5	XYZ@@com	Email Format Check	Err Msg
6	xyz@abc.com
Email Format Check	Valided Email ID
9	Abc12	Name can accept number	Valid Name
10	500	Digit	Valid digit or not


•	INTEGRATION TESTING
•	In Integration Testing we tested the system after integrating the unit testing’s successful modules.
•	We test each module that is dependent on other module. For e.g. Login Process Module, Registration Module, Option Module, Search List Module, etc.

•	SYSTEM TESTING
•	In this testing we take the requirements document as a reference to see whether the software meets all its requirements, goal or not.
•	The objective of the system testing is to promote software functionality, reliability and maintainability.

•	ACCEPTANCE TESTING
•	The system is demonstrated at the iTact Solutions, Surat There the system was tested.
•	Various realistic test data was provide by organization to test the system to be sure that the software is working satisfactory.

•	REGRESSION TESTING
•	Regression Testing will have to be performed when some changes will be made to an existing system.


9).	Limitations & System Enhancement
Limitations
	Device must have internet connectivity in order to use this application.
	Later updated records are impossible to remove/update at client.
	This system is only targeted towards for Entertainment.
	Only admin having rights of providing information.
	This application is only supported to Android devices.
	User must load all the data from server while installing application first time.
	Couldn’t support Multilanguage interface.
	
System Enhancement
	Try to introduce device independent application.
	Try to produce better user interface.
	Try to increase user interaction with server.
	Try to introduce feature using which admin can control system using mobile device.
 
10) References

Books
Beginning Android 2 by Mark L. Murphy

Websites
www.w3schools.com/php/default.asp

www.developer.android.com

www.android.com

www.androidpeople.com

www.stackoverflow.com

www.androidhive.info

www.findicons.com

	

This is the documentation of the apps
