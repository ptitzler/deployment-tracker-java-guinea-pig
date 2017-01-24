# deployment-tracker-liberty-guinea-pig
Test application for https://github.com/IBM-Bluemix/cf-deployment-tracker-client-java

### How to run

Download the sample application:

```
 $ git clone https://github.com/ptitzler/deployment-tracker-java-guinea-pig.git
 $ cd deployment-tracker-java-guinea-pig
``` 

By default two instances of this sample application will be started when you run `cf push`. Each instance sends a tracking request to the [Deployment-Tracker service](https://github.com/IBM-Bluemix/cf-deployment-tracker-service).

> Customize `manifest.yml` and `src/main/resources/META-INF/package.json` as desired to test specific scenarios or client versions.

Package, push and start the sample application:

```
 $ mvn clean package
 $ cf push
```

Open the sample application in a web browser and click the *View tracking status* link to review the tracking information.
