![[Pasted image 20260730211104.png]]
The application interacts with a number of external entities (actors) as shown on the following Context Diagram.

The actors include:

- **Student/User:** a person who accesses the application and interacts with fire safety scenarios. They make decisions during simulated emergency situations and receive feedback accordingly.
- **Authentication Provider:** a 3rd-party authentication and authorisation provider such as Google. 
- **Database:** the application uses an SQL database such as SQLite to store student progress, scenario outcomes, and session data.

The following is a shows a top level structure of the application.
![[Pasted image 20260730211543.png]]
Users must register and subsequently login with the application in order to save their progress. To register/login, users will need to provide valid third party credentials, for example Google. 

The user is given their in game progress, so that they can continue where they left off if playing for a second time. 