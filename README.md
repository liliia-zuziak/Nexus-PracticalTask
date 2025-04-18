# Practical Task Report: Nexus Setup and Artifact Deployment via Maven

## 1. Install Nexus
- **Version installed**: Sonatype Nexus Repository Manager 3.79.1-04  
- **Commands used**:
```bash
tar -xvf nexus-3.79.1-04-mac-x86_64.tar
cd nexus-3.79.1-04/bin
./nexus start
```
- **Result**:  


 ![alt text](<Screenshot 2125-04-17 at 12.01.32.png>)
**Extraction of the Nexus archive and folder structure creation.**

![alt text](<Screenshot 2125-04-17 at 12.04.16.png>)
**Starting the Nexus service using the `./nexus start` command.**

![alt text](<Screenshot 2125-04-17 at 12.06.03.png>)
**Nexus user interface is accessible via browser at `localhost:8081`.**
---

## 2. Configure Admin User
- **Result**:  
Admin user successfully logged in to the web interface.


![alt text](<Screenshot 2125-04-17 at 12.12.24.png>) 
_Logged in as the default `admin` user._

---

## 3. Configure Maven Proxy Repository

- **File modified**: `~/.m2/settings.xml`  
- **Configuration added**:

![alt text](<Screenshot 2125-04-17 at 12.28.43.png>)

![alt text](<Screenshot 2125-04-17 at 12.30.34.png>)

![alt text](<Screenshot 2125-04-17 at 12.30.44.png>)


---

## 4. Upload `spring-petclinic` Artifact to Nexus

### a. Add Maven Deploy Plugin to `pom.xml`

![alt text](<Screenshot 2125-04-17 at 12.37.30.png>)

![alt text](<Screenshot 2125-04-17 at 12.50.16.png>)
_The deploy plugin is added to the Maven build configuration to support artifact uploads._

![alt text](<Screenshot 2125-04-17 at 12.56.39.png>)

![alt text](<Screenshot 2125-04-17 at 12.47.51.png>)

![alt text](<Screenshot 2125-04-17 at 03.01.25.png>)
---


## 5. Search Artifact in Nexus

- **Result**:  


![alt text](<Screenshot 2125-04-17 at 03.05.13.png>)
