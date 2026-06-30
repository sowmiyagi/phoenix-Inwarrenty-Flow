#Postman API Automation Integration with Github Actions #

This repository is a demonstration of poc for integrating postman test with github actions. The tests are written in postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.

Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch.The projects run on a scheduled time with the help of the cron job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with they can view the report directly from the github page :https://sowmiyagi.github.io/phoenix-Inwarrenty-Flow/

## Tech Stack ##
1.Postman
2. Nodejs
3. Newman
4. Newman-reportor-htmlextra
5. Github Actions
6. Github pages

## How to run the Project? ##
You can run the project on your local system for that:
clone the project on your local machine : https://github.com/sowmiyagi/phoenix-Inwarrenty-Flow.git
Install Nodejs and NPM
Install Newman using npm install -g newman
Install newman-reportor-htmlextra npm install -g newman-reportor-htmlextra
Run the newman command 
  newman run 'In-Warranty collection Copy.postman_collection.json' \
          -e QA.postman_environment.json \
          -r cli,htmlextra \
          --reporter-htmlextra-export ./newman/index.html

