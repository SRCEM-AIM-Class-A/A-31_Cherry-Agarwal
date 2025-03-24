
## **Overview**  
This project is a Django-based multi-app web application designed for containerization and automated deployment.  

### **Technologies Used**  
- **Framework**: Django  
- **Containerization**: Docker  
- **Automation**: Jenkins  
- **Deployment**: Docker Hub  

## **Project Structure**  
```
StudentProject/  – Main Django project folder  
app1/            – Contains the homepage  
app2/            – Contains a sample page  
templates/       – Global templates for UI  
static/          – Contains CSS for styling  
Dockerfile       – Defines container setup  
Jenkinsfile      – Automates CI/CD pipeline  
```

## **Running the Project Locally**  
### **1. Clone the Repository**  
```bash
git clone  

**(https://github.com/SRCEM-AIM-Class-A/A-31_Cherry-Agarwal.git)**
```

### **2. Run with Docker**  
To run the project inside a Docker container, use:  
```bash
docker build -t studentproject .  
docker run -p 8000:8000 studentproject  
```  
Now, open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.  

## **Pulling from Docker Hub**  
Instead of manually building the image, you can pull the prebuilt version:  
```bash
docker pull agarwalcp/studentproject:latest  
docker run -p 8000:8000 agarwalcp/studentproject  

Your project will now be accessible at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).  

## **Jenkins CI/CD Pipeline**  
The Jenkins pipeline automates:  
1. Pulling the latest code from GitHub  
2. Building the Docker image  
3. Pushing the image to Docker Hub  

Any changes pushed to GitHub will automatically trigger the pipeline for continuous integration and deployment.  

## **Important Links**  
- **GitHub Repository**: [A-31_Cherry-Agarwal](https://github.com/SRCEM-AIM-Class-A/A-31_Cherry-Agarwal)  

## **Conclusion**  
This project showcases a complete CI/CD pipeline using Django, Docker, and Jenkins, ensuring automated builds, testing, and deployment following best DevOps practices. 🚀
