# task-07
# Task: GitHub Issue Integration for Internship Management System
## Documentation of GitHub Issue Integration for Internship Management System

Overview
This document confirms the successful completion of the GitHub issue integration task for the Internship Management System. The integration enables supervisors to assign GitHub issues along with tasks.

Completed Tasks
1. GitHub Handle Linking: Intern profiles updated to include GitHub usernames, with validation using the GitHub API.
2. Supervisor Task Assignment with GitHub Issues: Created task form extended to allow selection of GitHub issues, with fetching and display of open issues from linked repositories.
3. Data Storage: GitHub issue data stored alongside tasks, including Intern ID, GitHub Issue ID, issue title, issue URL, repository name, and date assigned.
4. GitHub Integration: GitHub REST API (v3) used to fetch repository issues, with secure storage of GitHub Personal Access Token (PAT) in `.env`.
5. User Interface: Task creation Blade view modified to include toggle for assigning GitHub issues, with dynamic loading of issues using AJAX.

## Usage
## For a super user, admin or a supervisor
a) Assigning a Task
    When a task is to be created, at the bottom of the form to be filled there is a checkbox to include a github issue. Once pressed it displays a dropdown of the available repositories on the organization’s github account to choose from.
    Once a repository is selected, we click on “Get Issues”, it then loads all the issues if any from the repository and displays them. One can select any issue he sees fit to. It was made so that multiple issues from different repositories can be selected
    Once selected and the form is ready, it can be submitted.
b) Viewing tasks
    When viewing the tasks it simply displays the assigned issues just under the task description where one can view the issue on github, one can also view the repository, and toggle any particular issue to either close or open state.
c) Viewing submissions
    Submissions on the task view page only includes the issues that were closed on submission, so does that on the submissions view page.
## For an intern or a worker
a) Viewing tasks
    When viewing the tasks it simply displays the assigned issues just under the task description where one can view the issue on github, one can also view the repository, and toggle any particular issue to either close or open state.
b) Submitting task
    When task is submitted it takes notes of the number of issues closed at the time the task is submitted
c) View Submission
    When viewing submission, it displays the issues after submission description but here one isn’t able to edit the state
d) Edit Submission
    On the edit submission page, one can edit the state of the issue
