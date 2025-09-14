# 🛠️ Maven Notes  

## 📖 What is Maven?  
- 🏗️ **Maven is a build automation and project management tool** primarily used in Java-based projects.  
- ⚙️ It helps manage a project's **build process, dependencies, documentation, and reporting**.  
- 📦 Maven uses a **Project Object Model (POM)** to define a project's structure and configuration, making it easier to handle **large and complex projects**.  
- 📑 The **pom.xml** file is the core of a Maven project → defines **project details, dependencies, plugins, and configurations**.  

---

## ⚡ Maven Build Lifecycle  

- `mvn compile` → 🏗️ Compiles source code.  
- `mvn test` → ✅ Runs tests.  
- `mvn package` → 📦 Creates artifact (`.jar` or `.war`) inside `target/`.  
- `mvn install` → 📂 Installs artifact into **local repo** (`~/.m2/repository/`).  
- `mvn clean` → 🧹 Deletes only the `target/` folder (not the `.m2` repo).  

---

## 📂 Local Repository  

- Installed artifacts go to 👉 `~/.m2/repository/...`.  
- `mvn clean` ❌ does **not** delete local repo.  
- To clear manually:  
  ```bash
  rm -rf ~/.m2/repository

🎯 Packaging Type

```<packaging>jar</packaging>``` → ⚙️ Maven creates .jar → Standalone app.

```<packaging>war</packaging>``` → 🌐 Maven creates .war → Deployable on servers like Tomcat.
