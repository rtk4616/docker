### Usage
#### Launch Jenkins master and its data container
```
docker-compose up
```

Rebuild
```
docker-compose rm -f
docker-compose pull
docker-compose up --build -d
```

Open http://localhost:8081/jenkins

#### Add Slave or angent
```
cd jenkins_slave;make build;make run url=<XXXX> secret=<YYYY>
```