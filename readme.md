# Log Monitor for Spring Boot Applications with Elastic Search and Grafana

This small demo project contains an example setup of ElasticSearch and Grafana to monitor Spring Boot applications.

The project contains a default Grafana ElasticSearch datasource and fetches data from application logs by using FileBeat

If you want to login to Grafana you can use the `admin / password` combination.


## Building the project

First build the spring boot application.

```bash
mvn clean package
```

Now when the application has been build we can start running our services by running:

```bash
docker-compose up
```

After all services have started successfully, you can navigate to the following urls:

- Spring Boot app - http://localhost:8080/
- ElasticSearch   - http://localhost:9092/
- Grafana         - http://localhost:3000/           