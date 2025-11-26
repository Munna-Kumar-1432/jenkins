🔥 What is Jenkins?
Jenkins is an automation tool used for CI/CD.
 Its job is to automatically build, test, and deploy your code.

⭐ Why is Jenkins important to learn?
CI/CD is used in almost every company


Developers don’t have to repeat manual tasks


Saves time


Code gets deployed fast and safely


Huge demand in the industry



🧠 Real Example of Jenkins
You pushed code to GitHub →
 Jenkins automatically:
Pulled the code


Created the build


Ran the tests


If everything is correct → deployed to the server


If anything is wrong → sends you an error on email/Slack


You might be sleeping, but Jenkins keeps working. 😄

📌 Jenkins Interview Questions (with Simple Answers)
✔ 1. What is Jenkins?
Ans: Jenkins is an automation tool used to create CI/CD pipelines.

✔ 2. What is CI/CD?
Ans:
CI (Continuous Integration): Automatically build/test whenever code is merged


CD (Continuous Deployment): Automatically deploy code to the server



✔ 3. What is a Jenkins Pipeline?
Ans:
 A script that defines steps like:
build


test


deploy


Example:
pipeline {
    stages {
        stage('Build') { ... }
        stage('Test') { ... }
        stage('Deploy') { ... }
    }
}


✔ 4. What is a Jenkinsfile?
Ans:
 A file where the pipeline script is written.
 It is stored in the repository.

✔ 5. What is a Jenkins Job?
Ans:
 A task in Jenkins. Like build job, test job, deploy job.

✔ 6. Why do we use plugins in Jenkins?
Ans:
 To add extra features.
 Examples: Git, Docker, AWS, Slack, SonarQube plugins.

✔ 7. What is a Freestyle Job in Jenkins?
Ans:
 A simple job where steps are added through the GUI.

✔ 8. What is a Declarative Pipeline?
Ans:
 A structured pipeline written in a Jenkinsfile.

✔ 9. How does Jenkins run automatically?
Ans:
 Through Webhooks.
 Push code to GitHub → Jenkins starts automatically.

✔ 10. What is Jenkins Master-Slave Architecture?
Ans:
Master: Controls everything (starts and manages jobs)


Slave/Agent: Runs the actual build


🔥 How to Create a Job in Jenkins? (Step-by-Step)
Step 1: Open Jenkins
Go to your browser and open the Jenkins URL:
http://localhost:8080


Step 2: Click on “New Item”
On the left side, you will see the New Item button → click on it.

Step 3: Enter the Job Name
Type the name of the job you want to create.
 Example:
My-First-Job


Step 4: Select Job Type
You will see options like:
Freestyle Project


Pipeline


Multi-branch Pipeline


Folder


If you want to create a simple/basic job, select Freestyle Project.

Step 5: Click on OK

Step 6: Job Configuration Page Opens
Here you can:
Add Git repository


Add build steps


Run commands


Set webhook or schedule



⭐ Simple Example: Git + Build Job
Source Code Management → Git
Enter your repository URL:
https://github.com/username/repo.git


Build Section → Add build step
Select:
Execute shell

Inside the shell, write:
npm install
npm run build

Then click Save.

Step 7: How to run the job?
Click the Build Now button on the top-right side.

Step 8: Check Console Output
On the left side, you will see Build #1 → click it →
 Open Console Output to see what’s happening.

⭐ Short Summary (Your Style)
Open Jenkins


Click New Item


Enter Job Name


Select Freestyle Project


Add Git repo


Add build steps


Save


Click Build Now


Check Console Output

🔥 What is a Job in Jenkins?
A Job in Jenkins is a task
 that tells Jenkins what work it has to perform.
When you create a Job, you give Jenkins the steps:
pull this code


create this build


run these tests


deploy this project


or run any shell command


In simple language:
 Job = Work assigned to Jenkins
 When Jenkins runs the job → it follows all the steps you gave.

⭐ Example (Simple)
If you create a job and write:
1. Pull code from Git
2. npm install
3. npm run build

Then Jenkins will automatically perform these 3 steps.
 This whole process happens inside a job.

🧠 Real-World Example
You created a job:
Build-App-Job
Inside this job, steps are:
Pull code from GitHub


Build the code


Run unit tests


Deploy to server


When you click Build Now →
 Jenkins performs all these tasks automatically.

📌 Short Definition (Interview Style)
Jenkins Job:
 A Jenkins job is a task that defines what Jenkins should do, such as building, testing, or deploying a project.


