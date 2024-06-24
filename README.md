# MyWebClass Collaboration and Brainstorming Assignment

## Overview

The purpose of this assignment is to practice collaborating using GIT/GitHub and develop the requirements for the mywebclass.org website's tutorials and courses.  To accomplish this task we are going to create three lists(What I Know, What I Don't Know, and What I Want To Learn) and consolidate the items from everyone in the class into a master list that counts the number of repeated issues.  You need at least **3 items for each list for a total of 9 items** and you should plan that these items are going to be used for project 1 as the basis for the possible topics that people can choose to build online tutorials about.   

## Learning Objectives:
1.  You will learn to collaborate online using GIT
2.  You will learn to merge pull requests and resolve merge conflicts
3.  You will learn to manage a basic project using GitHub Project.

### Complete the Assignment By adding your issues to these 3 lists and count how many times each issue is mentioned.  The number in the bracket next to each issue is the count, you should set your count at 1 for your issue.  We need the count of how many times the issue is mentioned, so that we can prioritze each issue.
## Put your items here
### Things you understand so far
1.  I understand how to push to github
2.  github conflict
3.  how to merge
4.  How to merge things even better
5.  I know how to use vim
6.  I know how to use bash scripts
### Things you don't understand about what we are doing
1. I am lost on hows to pro-Docker
2. I am lost on hows to pro-Linux
3. I am lost on hows to setup my domain name with my Oracle account
4. I am lost on hows pull for this assignment
5. I am lost on how to config
6. I am lost on what causes conflict
### Things you want to know next
1. setup domain name
2. why tedious assignment
3. I want to know how to resolve conflicts

### Your list should look like this:
#### Things we understand**
1.  Python Print[1]
2.  Linux Directory listing[2] 
3.  Docker Installation[1]
#### Things we don't understand
1. Git Stash[1]
2. GIt pull[2]
3. GIT status[1]
#### Things we want to know next**
1.  Elastic Search Indexing [1]
2.  Cloud deployment with Kubernetes[2]
3.  Teraform[1]

## Prerequisite - YOU. MUST SETUP PRIVATE PUBLIC KEY AUTH WITH GITHUB OR YOU WILL GET ACCESS DENIED ERRORS WHEN YOU PUSH FROM THE TERMINAL
Add your ssh public key to github - See video
**open powershell or terminal and run "ssh-keygen -b 4096" and hit enter through the prompts and then open the file **your home directory/.ssh/id_rsa.pub** and copy that text into your github account settings under SSH/GPG keys -> add key.  in one of the prompts it will tell you where it is going to save the key.  If you already have a key reusue the one you have and cancel out of the process with control c **.  I do it on my mac with the command vi ~/.ssh/id_rsa.pub" and then i press shift colon : and q to quit

### [Assignment Video](https://youtu.be/UFLKojO3OtM)

## You will accomplish this assignment in 5 phases:

1.  Each person will follow the instructions below to create one issue per list item i.e. 9 issues.
  **You need one issue per item in your list for a total of 9 issues.**.  Resolve each issue to add each of your items to the appropriate list.

2.  Find a person in class and then make a pull request for each item on your list to **THEIR** repository.  **You make 9 pull requests to someone else**

This person should then merge the pull requests and resolve the merge conflict to add new items to their list and increment the count on dupilicate items.  We want to know how many people said the same thing, so that we can prioritize the requirement, when we decide on what to make in project 1.  

3.  **Once you have merged the pull requests from someone else in class**, you need to find someone new in class to submit a pull request called "merge my list".  that asks to merge your master into their master, so that they can add new items to their list and increment the duplicate issue count for each item in the list.  Create an issue using the template "Assignment Master List" and reference the pull request that you make in the issue.  Make sure you make a issue template to accept this issue on your own repository and provide these instructions.

4. The person that receives the pull request from #3 needs to resolve merge conflics and merge, so that the new issues are added and duplicate counts are incrimented as necessary.

5. Once you have merged someone else's combined list into your project make an issue and a pull request to the "complete_list" branch on the upstream repository i.e. the one you forked from. Use the issue "Complete List" and put a link to the pull request.  Submit a link to the **issue** to Canvas to finish the assignment.  In your pull request include your UCID,  course number, and section.  

### You are done when you have completed the following:
 
1.  Added your issues individually and resolved them
2.  Made 9 pull requests to another person for each item that contains the branch you want to merge 
3.  Merged 9 pull requests from someone else
3.  Made a pull request to another person with your master branch that contains the consolidated list 
4.  Merged the pull request of someone elsesa compiled list
5.  Submmited a pull request to this repository to have your complete list merged

### Canvas Submission instructions

To submit this assignment you need to submit the result of step #5 to canvas.  When you look at the commits for your project you should see a total of 3 different users have contributed items to the list **including yourself** .  If you don't have at least 3  people's commits on the project you will lose 33 points for each person not found.

## Project Setup Instructions
Collaborating on GitHub:

1. Fork the repository: Each person should fork the repository to their own GitHub account. To do this, click the "Fork" button in the top-right corner of the repository page.
2. Enable issues: If you don't see the "Issues" tab in the main menu, you should enable it in the repository settings. 
3. Go to the "Issues" tab, and click "Milestones" to add a 0.1.0 milestone and describe it as a consolidated list of issues from your team.  
4. Go to the issues tab you should also create labels for "I Know", "Want to Know", "Don't Understand", and "Master List".  
5. Once you create these labels then go to settings and look for the "Issues Template" and create/edit 4 issue templates that will provide the starting text for each issue filed of that type.  At the bottom of each issue you will see that you can automaticly assign a label to that issue type, so connect the respective labels you created with the 4 issue types.  You need an issue for "I Know", "Want to Know", "Don't Understand", and "Master List".
4. Goto the project tab and create a new project (you have to click the down arrow next to "link project" to change it to new project). When you create a project you need to select "board" and name it "Documentation Tasks".
5. Once this is completed then clone this to your computer using the SSH link **NOT THE HTTP LINK** you need the ssh link to use the key you added to your account, so you don't get an error when pushing.


### Project management and Collaboration workflow Steps
1. create an issue
2. assign issue to project task
*  Assign to yourself
*  Assign to correct project board
*  Assign to "todo" project status
*  Assign to the correct milestone
* create issue branch 
3.  Go to the project board and move the task you created to in progress
4. git fetch origin to see new branch
5. checkout issue branch locally
6. git status to make sure you don't have any changed files in the branch before you work
7. Resolve the issue by adding the list item or incrementing the count of the item
8. commit -a -m "message text" to do the commit 
9. git push origin head <- pushes current branch to github
10. Do a pull request for the branch and make sure you pick the correct source and destination.  Click compare forks because by default it will go to the upstream repository i.e. mine
11.  merge the pull request and add "closes #<issue number> i.e. closes #4 to close the issue
12.  Check that your task is moved from in progress to done
13.  update your local main branch with the changes from the merge by doing git pull origin main
14. Repeat again, and again, and again

<<<<<<< HEAD
=======
1. Add items to the list
=======
1. I know how to make ssh keys
<<<<<<< HEAD
>>>>>>> 2716e3e74f642aa96b78a25883d4471db75400fd
=======
2. I know personal domain use
<<<<<<< HEAD
>>>>>>> 515aa38a7113dc8aa753aa4d7bbf4b14fc3e326a
=======
3. I know how to make a personal token
>>>>>>> 028a10787611c0b89a8972e44f171a76ac36db22
### Things you don't understand about what we are doing / web development.
1. Don't understand forking
2. Don't Understand Oracle Cloud
3. Don't understand the difference between cloning and forking
### Things you want to know next
<<<<<<< HEAD
1. How to connect viewjs to elastic search
2. This is something I want to know
>>>>>>> f64d4009149766f89d55a555333912054e9062d6
=======
<<<<<<< HEAD
### Joshua Kaisar's List:
#### Things we understand**
1. How to make a static website
2. Git
3. Agile
4. Docker

#### Things we don't understand
1. Difference between Scrum and Kanban
2. Terraform Automation
3. Kubernetes

#### Things we want to know next**
1. Microsoft Azure
2. AWS S3 Buckets
>>>>>>> f4f4c33a292f0d792ab74f3e879a71ccf9197e9d
=======
1. More in depth SQL
>>>>>>> 8b44ab78b09b81220e9d9c5d4970d14755c6eb13
>>>>>>> 78a4abf81071b0d5e7b669da13dde65c901fbc12

test