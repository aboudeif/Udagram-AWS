### **Pipeline process**
![Pipeline diagram](/screenshots/pipeline-daigram.png?raw=true "Optional Title")

## Pipeline process

* First install node and checkout code
* then setup aws-cli
* use root level package.json to install dependencies in the frontend app

 1- Build job
  * Install API dependencies
  ```
  npm run api:install
  ```
  * Install Frontend dependencies
  ```
  npm run frontend:build
  ```
  * Build API
  ```
  npm run api:build
  ```
  * Build Frontend
  ```
  npm run frontend:build
  ```

 2- Deploy job
  * Deploy both forntend and API using
  ```
  npm run api:deploy && npm run frontend:deploy
  ```
