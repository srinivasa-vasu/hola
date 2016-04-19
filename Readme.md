# hola
Hello microservice using Java EE (JAX-RS) on WildFly Swarm

Build and Deploy hola
---------------------

1. Open a command prompt and navigate to the root directory of this microservice.
2. Type this command to build and execute the application:

        mvn wildfly-swarm:run

3. This will create a uber jar at  `target/hola-swarm.jar` and execute it.

Access the application
----------------------

The application will be running at the following URL: <http://localhost:8080/api/hola>

Deploy the application in Openshift
-----------------------------------

1. Make sure to be connected to the Docker Daemon
2. Execute

		mvn clean package docker:build fabric8:json fabric8:apply