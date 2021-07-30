# EHI_Project_Salman

CONTACT DEMO 

By Syed Salman Ahmed Hashmi
Date 30 July 2021


Project Description:

Design and implement a production ready application for maintaining contact information. 

Expected functionality:
- add a contact
- list contacts
- edit contact
- delete contact

Required Contact model:
- First Name
- Last Name
- Email
- Phone Number
- Status (Possible values: Active/Inactive)

Environment Required to run:

1) Microsoft Visual Studio Express 2019 for web ( as .Net Core is not supported in VS2017 or lower
	-.Net Core 5.0
2) Microsoft SQL Server 2017 (RTM) - 14.0.1000.169 (X64) 

For DB please find script in DatabaseScripts folder of project
Change DefaultConnection value in ContactDemoAPI/appsettings.json to the new database server. 
Current value of above should be "Server=INMD2009LL0320\\SQLEXPRESS;DATABASE=ContactDemoDB;Trusted_Connection=True;MultipleActiveResultSets=true"


About the API:

Technology used ASP.NET CORE 

Traget Framework: v5.0

Architechture: Nteir
-BO for business validation (checked for valid contactID and Status)
-DAO - to connect to DB and perfor CRUD operations
-DTO - holds the entities

Dependencies
ContactDemoAPI :- ContactDemoBO, ContactDemoDTO
ContactDemoBO :-ContactDemoDAO, ContactDemoDTO
ContactDemoDAO :- ContactDemoDTO


DB: MSSQL

ThirdParty AddIns

Dapper - SQL operations
Swagger - API UI for testing




