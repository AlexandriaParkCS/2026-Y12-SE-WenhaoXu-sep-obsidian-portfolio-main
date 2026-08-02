![[Pasted image 20260730230151.png]]
Game Loading process
The Dashboard Generation process is responsible for presenting each student's personalised progress summary within the application. This process is initiated when a student completes a scenario or returns to the main menu to review their progress.

At the top of the hierarchy is the Load game module, which coordinates all submodules to retrieve, process, and present relevant progress data. It delegates tasks to two key modules: Get User Data and Get Progress. Get User Data is responsible for verifying the student's identity by exchanging credentials, while Get Progress uses the student's User ID to query the database and retrieve a list of completed levels.

Once data is retrieved, it is passed back to the Generate Dashboard module, which compiles and displays the student's progress summary, showing which scenarios have been completed and any feedback or scores associated with them.
