## BUILDING DOCKER IMAGE
```commandline
Get base image from docker registry

it starts with FROM "to declare base image"

2. Declare working DIRECTORY of DOcker
    
    " WORKDIR /app"
    
3. DEcalraing dependencies ====
     click package.jsom
     "COPY package.json . or /app"
     
4 TO install dependencies and libraries we use eg
  "RUN npm install"
  
Expose port by mapping an external port to the internal port

CMD command 

```
## DOCKER 
```
GO to your VM == sudo su
GO to github copy your code url
Go to VM and run " git clone <paste url>
docker build -t feedback-node . ### -t provide the name of the app e.g "feedback-node
docker build -t feedback-node:v2 .

```
## DOcker PUSH

```commandline
First create a repo in docker hub with the same app name

docker login --username ibbriggs

Dockerhub passwd TO0NIMI2021#eaPrime
```
## docker tag
```commandline
 docker tag  af34e9a57d2e ibbriggs/feedback-node:v3
            [image id]      [username/reponame]:tag or version
```
## DOCKER RUN 
```commandline
docker run -p 3000:80 --name (name of app) feedback-app -d (image name) ibbriggs/feedback-node:v3

```