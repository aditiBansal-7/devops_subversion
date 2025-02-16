 **Subversion (SVN) & Mercurial (hg) - Version Control Guide**

This repository demonstrates the usage of **Apache Subversion (SVN)** and **Mercurial (hg)** for version control, including installation, basic commands, troubleshooting, and hosting a project using **GitHub Pages**.

 ---

📌 **Introduction**
Version control systems are essential tools for managing code changes, collaborating with teams, and maintaining project history. This guide covers:
- **Subversion (SVN)** – A centralized version control system.
- **Mercurial (hg)** – A distributed version control system.

Both tools help developers efficiently manage and track changes in their projects.

---

🚀 **Installing Subversion (SVN)**

### **Windows Installation**
1. Download **VisualSVN Server** from [here](https://www.visualsvn.com/server/download/).
2. Run the installer and follow the setup wizard.
3. Install **TortoiseSVN** (GUI client) from [here](https://tortoisesvn.net/downloads.html).
4. Restart your system to apply changes.
5. Verify installation using:
   ```sh
   svn --version
   ```

---

🔧 **Using Subversion (SVN)**

1️⃣ **Clone an SVN Repository**
```sh
svn checkout <repository_url> my_project
```
✅ This command creates a local working copy of the repository.

2️⃣ **Navigate into the Repository**
```sh
cd my_project
```

3️⃣ **Add New Files**
```sh
svn add myfile.txt
```
✅ Adds a new file to version control.

4️⃣ **Commit Changes**
```sh
svn commit -m "Added a new file"
```
✅ Saves changes to the repository with a message.

5️⃣ **Update the Repository**
```sh
svn update
```
✅ Retrieves the latest changes from the remote repository.

6️⃣ **Push Changes to Remote**
```sh
svn commit -m "My updates"
```
✅ Uploads committed changes to the repository.

---

🚀 **Installing Mercurial (hg)**

 **Windows Installation**
1. Download Mercurial from [here](https://www.mercurial-scm.org/downloads).
2. Run the installer and follow the setup wizard.
3. Verify installation:
   ```sh
   hg --version
   ```

---

🔧 **Using Mercurial (hg)**

1️⃣ **Clone a Repository**
```sh
hg clone <repository_url> my_project
```
✅ Creates a local copy of the repository.

2️⃣ **Navigate into the Repository**
```sh
cd my_project
```

3️⃣ **Edit Files & Add Changes**
```sh
hg add myfile.txt
```
✅ Adds new or modified files to be tracked.

4️⃣ **Commit Changes**
```sh
hg commit -m "My first commit"
```
✅ Saves changes to the local repository.

5️⃣ **Push Changes to Remote**
```sh
hg push
```
✅ Uploads committed changes to the remote repository.

---

⚠ **Common Errors & Troubleshooting**

🔹 **SVN Authorization Failed**
**Error Message:** `Authorization failed`
**Solution:**
- Verify your **username & password**.
- Check if you have **write permissions**.
- Use:
  ```sh
  svn auth --store-passwords=yes
  ```

🔹 **Mercurial Push Authorization Failed**
**Error Message:** `abort: authorization failed`
**Solution:**
- Check if the **remote repository is accessible**.
- Ensure correct authentication:
  ```sh
  hg push --config auth.x.username=<your-username>
  ```

---




👤 **Author**
**Name:** Aditi Bansal  
**Roll Number:** 500106987  
**Student ID:** R2142220221  

---

