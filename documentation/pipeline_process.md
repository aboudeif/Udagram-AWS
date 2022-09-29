### **Pipeline process**
![Pipeline diagram](/screenshots/pipeline-daigram.png?raw=true "Optional Title")

## Pipeline process

* first install node and checkout code
* then setup aws-cli
* use root level package.json to install dependencies in the frontend app

 1- job one (Build)
  * npm run api:install
  * npm run frontend:build
  * npm run api:build

 2- job two (Deploy)
  * npm run deploy
  ```
  npm run api:deploy && npm run frontend:deploy
  ```
