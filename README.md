# docker-workshop env Vorbereitung
```
cd /home/user
mkdir projects
cd projects
git clone https://github.com/iScraM12/rover-service.git
git clone https://github.com/iScraM12/rover-ui.git
git clone https://gitlab.com/twn-youtube/docker-compose-crash-course.git
```

```
cd rover-service
mvn clean package
docker build -t rover-service .
cd ..
```

```
cd rover-ui
npm install && npm run build
docker build -t rover-ui .
cd ..
```
