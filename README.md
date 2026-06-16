# Sausage Store

![image](https://user-images.githubusercontent.com/9394918/121517767-69db8a80-c9f8-11eb-835a-e98ca07fd995.png)


## Technologies used

* Frontend – TypeScript, Angular.
* Backend  – Java 16, Spring Boot, Spring Data.
* Database – H2.

## Installation guide
### Backend

Install Java 16 and maven and run:

```bash
cd backend
mvn package
cd target
java -jar sausage-store-0.0.1-SNAPSHOT.jar
```

### Frontend

Install NodeJS and npm on your computer and run:

```bash
cd frontend
npm install
npm run build
npm install -g http-server
sudo http-server ./dist/frontend/ -p 80 --proxy http://localhost:8080
```

Then open your browser and go to [http://localhost](http://localhost)

```
kubectl get pods -n r-devops-magistracy-project-2sem-1470092013
NAME                                            READY   STATUS      RESTARTS        AGE
mongodb-0                                       1/1     Running     0               28m
mongodb-init-reports-kjbxb                      0/1     Completed   0               45s
postgresql-0                                    1/1     Running     0               28m
sausage-store-backend-59949459df-wgkcv          1/1     Running     0               11m
sausage-store-backend-report-57dd89cdcb-thkn2   1/1     Running     7 (5m40s ago)   11m
```