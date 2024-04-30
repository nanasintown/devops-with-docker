````bash

```sol1_8 % docker build . -t web-server
Sending build context to Docker daemon  2.048kB
Step 1/2 : FROM devopsdockeruh/simple-web-service:alpine
 ---> fd312adc88e0
Step 2/2 : CMD server
 ---> Running in f07496303de7
Removing intermediate container f07496303de7
 ---> d897b2244754
Successfully built d897b2244754
Successfully tagged web-server:latest

Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them


mac@nanasmac sol1_8 % docker run web-server
[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
 - using env:	export GIN_MODE=release
 - using code:	gin.SetMode(gin.ReleaseMode)

[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
[GIN-debug] Listening and serving HTTP on :8080
````
