# Assignment –1

## DevOps

### By 
Aditi Bansal 
500106987
R2142220221 

---

## Mercurial: Using Mercurial (hg) for Version Control

### Introduction
Mercurial is a distributed version control system that allows developers to track changes in their code and collaborate with others. This document outlines the steps to clone a repository, make changes, and push those changes back to the remote repository using Mercurial.

---

## Steps to Clone a Repository and Push Changes

### Step 1: Clone the Repository
To clone a repository, use the following command:

sh
hg clone <repository_url> hello


Explanation: This command creates a local copy of the repository located at the specified URL. The local copy will be created in a directory named hello.

### Step 2: Change Directory
Navigate into the cloned repository directory:

sh
cd hello


Explanation: This command changes the current working directory to the hello directory, where the cloned repository resides.

### Step 3: Edit Files
Make the necessary changes to the files in the repository. You can use any text editor or Integrated Development Environment (IDE) of your choice to edit the files.

### Step 4: Add New Files
If you have created new files or modified existing files, you need to add them to the staging area using the following command:

sh
hg add <file_name>


### Step 5: Commit Changes
Once you have added the files, commit your changes with a descriptive message:

sh
hg commit -m "My changes"


Explanation: The -m flag allows you to include a commit message that describes the changes you made. Replace 'My changes' with a meaningful message that reflects the nature of your changes.

### Step 6: Push Changes
Finally, push your committed changes back to the remote repository:

sh
hg push


Explanation: This command uploads your local changes to the remote repository, making them available to others.

---

### Common Errors and Troubleshooting

#### abort: authorization failed
This error message indicates that Mercurial is unable to authenticate your credentials when trying to push changes to the remote repository. Here are some common reasons for this issue and how to resolve them:

- Access Permissions: Check if you have the necessary permissions to push to the repository. If you are trying to push to a repository that you do not own or do not have write access to, you will receive an authorization error.
- If you are collaborating on a project, confirm with the repository owner that you have been granted the appropriate access rights.

---

End of Document
