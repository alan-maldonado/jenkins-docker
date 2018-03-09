# jenkins-docker

Clone this repo
```bash
git clone https://github.com/alan-maldonado/jenkins-docker.git
```

Change directory
```bash
cd jenkins-docker
```

Build docker image
```bash
docker build -t jenkins-docker .
```

Create docker container sharing docker
```bash
docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --name jenkins -d jenkins-docker
```
