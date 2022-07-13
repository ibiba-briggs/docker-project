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