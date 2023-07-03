# SPM SQL
CREATE SCHEMA INSTANCE;

CREATE TABLE SPM.INSTANCE.`Company Dimension Table` ( 
	Company ID int64 NOT NULL  ,
	Name string  
 );

CREATE TABLE SPM.INSTANCE.`Doctor Dimension Table` ( 
	Doctor ID int64 NOT NULL  ,
	First Name string  ,
	Last Name string  ,
	State string  ,
	Specialty string  ,
	Rating numeric  
 );

CREATE TABLE SPM.INSTANCE.Entity ( 
 );

CREATE TABLE SPM.INSTANCE.`Ratings Fact Table` ( 
	Doctor ID int64 NOT NULL  ,
	CMS rating numeric  ,
	RateMD Rating numeric  
 );

CREATE TABLE SPM.INSTANCE.`State Dimension Table` ( 
	State ID int64 NOT NULL  ,
	State Name string  
 );

CREATE TABLE SPM.INSTANCE.`Grants Fact Table` ( 
	Doctor ID int64 NOT NULL  ,
	Company ID int64 NOT NULL  ,
	State ID int64 NOT NULL  ,
	Number of Grants int64  ,
	Amount of Grants int64  
 );
