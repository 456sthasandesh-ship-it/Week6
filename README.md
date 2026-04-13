GitHub Version Control and Code Changes for Hotel Reservation System
Introduction

This README explains the steps I took to complete the Week 6 activity for the ICT272 Web Design and Development course. The goal was to practice using GitHub for version control, upload a project, make changes to the code, and document the process in a video presentation.

Step 1: GitHub Account Setup
I created a GitHub account at GitHub
 and logged in using my credentials.
This allowed me to manage my code, collaborate with others, and track project history.
Step 2: GitHub Desktop Installation
I downloaded and installed GitHub Desktop from GitHub Desktop
.
This software provides a graphical interface to manage repositories and commit changes to code.
Step 3: Uploading Previous Program
I uploaded the Hotel Reservation System project from my local machine to GitHub.
Created a new repository and pushed my files using GitHub Desktop.
Step 4: Code Changes
Change 1: Improved Input Validation

Before:

NumberOfnight = int.Parse(Console.ReadLine());

After:

int NumberOfnight;
while (!int.TryParse(Console.ReadLine(), out NumberOfnight))
{
    Console.WriteLine("Enter valid number:");
}
Explanation:
I replaced int.Parse with int.TryParse to prevent the program from crashing if the user enters invalid input. It ensures safer input handling.
Change 2: Improved Exit Condition

Before:

if (choice == "q" || choice == "Q")

After:

if (choice.Trim().ToLower() == "q" || choice.Trim().ToLower() == "exit")
Explanation:
I made the exit condition more flexible by allowing multiple variations of the exit command, such as "exit" or "quit", and trimming unnecessary spaces.
Step 5: GitHub Commit and Push
After making the changes, I committed them using GitHub Desktop and pushed them to the repository.
This allows me to keep track of all the modifications I made in my project.
Step 6: Reflection on the Process

From this activity, I learned how to use GitHub for version control. It helps in managing project versions, tracking changes, and collaborating with others. By using GitHub Desktop, I was able to manage the repository visually, making it easy to commit, push, and track code changes. This is an essential skill for real-world software development, especially when working with teams.
