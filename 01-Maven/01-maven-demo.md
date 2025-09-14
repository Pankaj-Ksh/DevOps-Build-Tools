# 🚀 Project: Maven-based Java Application on AWS EC2  

A simple Java application **hello-maven** built and deployed using **Maven** on an **AWS EC2 instance**.  
The project demonstrates a **manual CI/CD-like workflow**, covering **cloning, compiling, packaging, installing, and cleaning** a Maven project.  
It highlights the **integration of GitHub, Maven, and AWS EC2** in a development workflow.  

---

## 🎯 Objective  

- ✅ Set up a **Java-Maven development environment** on AWS EC2.  
- ✅ Demonstrate **GitHub → EC2 → Maven build pipeline**.  
- ✅ Build and package a **Java JAR file** using Maven.  
- ✅ Understand the use of **Maven lifecycle commands** (compile, test, package, install, clean).  

---

## 🔄 Workflow Summary  

1. 📂 **Set up GitHub Repository (hello-maven)** – Created repo with `src/` folder and `pom.xml`.  
2. 🌐 **Launched AWS EC2 Instance (Maven-server)** – Configured and accessed securely via SSH.  
3. ⚙️ **Installed & Verified Tools** – Git, Java (JDK), and Maven ready for development.  
4. ⬇️ **Cloned Project & Executed Maven Lifecycle** – Successfully ran `compile`, `test`, `package`, `install`.  
5. 📦 **Built & Installed JAR File** – Packaged `hello-maven` app and installed into local Maven repo.  
6. 🧹 **Performed Clean Build** – Used `mvn clean` to reset project to fresh state.  

---

## 🛠 Steps Performed  

📸 **Screenshots Explained:**  

1. **GitHub Repository Overview**  
   - Shows the `src/` folder and `pom.xml` file in the repo.  
   - Starting point for source code management.  
     <img width="1920" height="1032" alt="Screenshot (1553)" src="https://github.com/user-attachments/assets/1f9510f9-8ccb-4530-92cb-17281faf2fd2" />

2. **App.java**  
   - Simple Java class with a `main` method.  
   - Prints: `"Hello, Maven! This project is running successfully 👋"`.  
     <img width="1920" height="1034" alt="Screenshot (1554)" src="https://github.com/user-attachments/assets/8897b0cc-7402-4c56-b8ee-16bd4eb6eba4" />

3. **pom.xml**  
   - Contains project metadata (groupId, artifactId, version).  
   - Defines Maven dependencies and build configuration.  
     <img width="1920" height="1032" alt="Screenshot (1555)" src="https://github.com/user-attachments/assets/18b5d180-7669-4a9d-8d9f-447fbab3bd9c" />

4. **AWS EC2 Instance**  
   - Running instance named **Maven-server**.  
   - Public IP visible for remote access.  
     <img width="1920" height="979" alt="Screenshot (1557)" src="https://github.com/user-attachments/assets/944c9ae5-8bd7-44a4-af59-b4fff586fad0" />

5. **SSH Login**  
   - Shows login as `ec2-user` on EC2.  
   - Confirms successful remote connection.  
     <img width="1920" height="1080" alt="Screenshot (1558)" src="https://github.com/user-attachments/assets/5304316a-7baa-419a-879f-ba6ff4036329" />

6. **Software Versions**  
   - Verified installation of Git, Java, Maven.  
   - Ensures environment is ready for builds.  
     <img width="1920" height="1080" alt="Screenshot (1559)" src="https://github.com/user-attachments/assets/4bfc4c47-b850-4a41-b3dd-96629ffcc09f" />

7. **Git Clone**  
   - Cloned `hello-maven` repo from GitHub.  
   - `ls` confirms successful download.  
      <img width="1920" height="1080" alt="Screenshot (1560)" src="https://github.com/user-attachments/assets/987b0b43-af0f-4b9a-b043-12f8e22c2b99" />

8. **Maven Compile**  
   - `mvn compile` generated `.class` files.  
   - Verified inside `target/classes`.  
     <img width="1920" height="1080" alt="Screenshot (1561)" src="https://github.com/user-attachments/assets/640037ca-b8e5-4981-af12-6f19dfdbd10c" />

9. **Maven Test**  
   - Ran `mvn test` command.  
   - No test cases present, executed cleanly.  
     <img width="1920" height="1080" alt="Screenshot (1562)" src="https://github.com/user-attachments/assets/22090ff6-625f-4c74-bc83-2044a27a6ecb" />

10. **Maven Package**  
   - Packaged project into `.jar` file.  
   - JAR located in `target/`.  
     <img width="1920" height="1080" alt="Screenshot (1563)" src="https://github.com/user-attachments/assets/a9dfbbdd-f76b-40d8-b06b-1c9ee6253d14" />

11. **Maven Install**  
   - Installed JAR into local Maven repo.  
   - Available for reuse by other projects.  
     <img width="1920" height="1080" alt="Screenshot (1564)" src="https://github.com/user-attachments/assets/987b9ee1-90fe-4c29-9339-496a361442ab" />

12. **File Listings**  
   - `ls` shows project files and JAR in repo.  
   - Confirms build artifacts exist.  
     <img width="1920" height="1080" alt="Screenshot (1565)" src="https://github.com/user-attachments/assets/afb50bb1-eb38-4b13-a979-c9072bf442be" />

13. **Maven Clean**  
   - `mvn clean` removed `target/` folder.  
   - Project reset to initial state.  
     <img width="1920" height="1080" alt="Screenshot (1566)" src="https://github.com/user-attachments/assets/f5cc076b-d3b5-4ea9-836a-912d80a1f180" />

---

## ✅ Outcome  

- 🏗️ Successfully **built and packaged** a Maven-based Java application.  
- 📦 Generated and **installed JAR file** into local repository.  
- 🌍 Verified end-to-end workflow: **GitHub → EC2 → Maven lifecycle**.  
- 🧹 Learned how to **reset builds** using `mvn clean`.  

---

## 📚 Key Learnings & Observations  

- 🔑 **Maven lifecycle phases** (compile → test → package → install → clean).  
- 📂 **Target directory** is auto-generated to store compiled `.class` files and JARs.  
- 🔄 **`mvn clean`** helps ensure fresh builds without old artifacts.  
- ☁️ **AWS EC2** provides scalable and isolated dev environments.  
- 🛠️ **pom.xml** acts as the **blueprint** for project build and dependencies.  

---

## 🌍 Real-World Use Case  

- 🏢 Used in enterprises for **CI/CD pipelines** (Jenkins + Maven + GitHub + AWS).  
- 🔄 Helps automate **build, test, and deploy** of applications.  
- ⚙️ Common setup for **microservices development**, where each service is packaged as a JAR/WAR.  
- 🌐 Foundation for **DevOps pipelines** integrating tools like Docker, Kubernetes, and Cloud services.  

---

## 🏷️ Tags  

`#Maven` `#Java` `#AWS` `#EC2` `#DevOps` `#CI/CD` `#GitHub`  

---

## 💡 Tips  

- ✨ Always **verify versions** of Git, Java, Maven before starting builds.  
- 📝 Keep `pom.xml` clean and well-structured – it defines the project.  
- 🔄 Use **`mvn clean`** before packaging to avoid stale artifacts.  
- ☁️ Use **IAM roles** for EC2 authentication instead of long-term keys.  
- 🚀 Automate steps later using **Jenkins or GitHub Actions**.  

---
