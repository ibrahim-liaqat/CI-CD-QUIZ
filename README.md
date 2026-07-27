<div align="center">
  <h1>🚀 CI/CD Pipeline Project</h1>
  <p><i>A complete Continuous Integration and Continuous Deployment pipeline using GitHub, Jenkins, and Tomcat.</i></p>
</div>

---

## 💡 How it works

1. 💻 **Make changes** in the code and push them to GitHub.
2. 🔄 **Jenkins automatically detects** the changes.
3. ⚙️ **Jenkins builds and tests** the project.
4. 🌐 **Tomcat deploys** the latest version, and the website reflects the changes automatically.

---

## 🛠️ Pipeline Setup Steps

### 1️⃣ Link Jenkins to your Git Repository
🔗 In your Jenkins job, configure the Source Code Management to point to your GitHub repository.

### 2️⃣ Execute Build Commands in Jenkins
👨‍💻 In the Jenkins build configuration terminal (*Execute shell* or *Windows batch command*), add the commands to compile, run, and package your Java application.

**Compile and run the Java file:**
```bash
javac YourJavaFile.java
java YourJavaFile
```

**Command to make it a jar file:**
```bash
jar cvf YourApp.jar *
```

### 3️⃣ Deploy to Tomcat
📂 Make sure you copy the generated jar file into the Tomcat `webapps` (webpages) folder. Add this command to the Jenkins terminal:
```bash
cp YourApp.jar /path/to/tomcat/webapps/
```

### 4️⃣ Trigger Automatic Deployment
🚀 When you make a commit in GitHub, Jenkins will detect the changes automatically. It will run the commands configured in steps 2 and 3, which will then reflect the changes on your Tomcat local server.

---

<div align="center">
  <b>Built with ⚙️ Git, 🏗️ Jenkins, and 🐱 Tomcat</b>
</div>
