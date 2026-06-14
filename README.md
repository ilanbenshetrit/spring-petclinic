# Spring PetClinic — JFrog DevSecOps Pipeline

## מה הפרויקט
אפליקציית Java המריצה pipeline אוטומטי עם JFrog Artifactory ו-XRay.

## Pipeline
- קימפול עם Maven
- הרצת טסטים אוטומטיים
- בניית Docker image
- דחיפה ל-JFrog Artifactory
- סריקת אבטחה עם XRay

## הגדרת Secrets ב-GitHub
| Secret | תיאור |
|--------|--------|
| JF_URL | https://yourname.jfrog.io |
| JF_ACCESS_TOKEN | Access Token מ-JFrog |
| JF_USERNAME | המייל שלך ב-JFrog |
| JF_DOCKER_REPO_HOST | yourname.jfrog.io |

## הרצת ה-Image
```bash
docker pull trialf51g5s.jfrog.io/docker-local/spring-petclinic:TAG
docker run -p 8080:8080 trialf51g5s.jfrog.io/docker-local/spring-petclinic:TAG
```
