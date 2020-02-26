# Worldfavor recruitment test

## Introduction
This repository is for Worldfavor's developer candidates only.

Candidates are required to go through the different assignments by providing their own implementation. 

A review meeting shall be held after receiving the candidate's code; questions may be asked regarding the code and the mindset displayed in the implementation.

Plagiarism and collaboration are not only unethical but strongly discouraged. We ask that you clone the repo to your local disk and submit it back in a zip file to mitigate this. When zipping and sending us your work, please exclude the folder containing installed packages to reduce the size of the zip file.

This test should take no longer than 4h.

If you feel you did not have the time to complete all the assignments and show all your capabilities, please submit your response for evaluation as the test is designed to asses various skill levels.

How to implement the different scenarios is open to the candidate unless stated otherwise.

Be as true to yourself as you can, and good luck!

## Assignment
Your are asked to create and API which will take a CSV file as input and save the data into the database. Along with this you also need to create an endpoint which lets you read the saved data with various filters. 

You need to create the project structure and architecture necessary to achieve this. To us, implementation design is as important as solving the assignment.

### API endpoints
1)	__Import__: This endpoint will consume a file of type CSV, parse it and save the uploaded data to database and respond with a reply message i.e. if succeded response will be 200, if errors then response will contain what error 
have occurred
2)	__GetWith__: Endpoint will take a request object with filters (Name, Departments etc.) and return results from database.

### Data to import
The data file is in CSV format and is included in this repo.
   
### Technology Stack Required
- .NET Core 3.1
- ASP.NET Core 2.2 or above for API.
- Entity Framework Core for Database mapping with Code First Approach.
- SQL Server Express or MySQL as data storage.
- NUnit for TDD.

### Acceptance Criteria
1)	User should successfully upload a CSV file.
2)	Duplication of data should be prevented i.e each employee in Db needs to be unique Employee Number in case the data is present update operations should be performed and relevant message should be shown in reply.
3)	API should be RESTFul and return a solid JSON structure.
4)	Unit testing should be performed on all layers of application.
5)	Integration testing needs to performed to check all use case flows.
6)	Application should be based on principles of solid separation of concerns and should implement design patterns for database operations, API operations choice of these are up to your best knowledge.

### Bonus Points
1)	Leveraging of DOI Containers
2)	Exception handling
3)	Logging
