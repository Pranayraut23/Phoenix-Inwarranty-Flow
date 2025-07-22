# Postman API Automation Integration with Github Actions #

This repoistory is a demonstration for POC for integreating postman tests with github actions. The tests are written in postman and they are executed on VM with the help of newman and newman-reporter-htmlextra.
Github actions will trigger the project execution on every push to the main branch. you can also execute project manually using workflow_dispatch. The projects runs on a scheduled time with the help of cron job.

The HTML report is acrchieved and kept in the artifact section forthe team to download. Along with that they can view the report directly from the github page: https://pranayraut23.github.io/Phoenix-Inwarranty-Flow/
The latest report is mailed to the team members using Gmail SMTP

## About Me ##
Hi My Name is Pranay Raut. I have 7 years of experience in QA Automation Testing . My Skill sets includes UI automation with seleniuem webDriver and for API testing i used Rest Assured and Postman.
You can connect with me over : (https://www.linkedin.com/in/pranayraut23/)

## Testing Coverage ##
1. Happy flow testing
2. Negative Testing and Edge case Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets management using Github Secrets


## Tech Stack ##
1.Pstman
2.Nodejs 22V
3.Newman
4.Newman-Reporter-Htmlextra
5.GitHub Actions
6.Gmail SMTP
7.Github pages
8.CSV for Data Driven Testing
9.AWS-EC2 instance for self hosted github runner

## Github Pages ##
You can directly view the latest test reportof the Postman Test at : https://pranayraut23.github.io/Phoenix-Inwarranty-Flow/

## HTML Report ##
The report will be created in the newman folder
![Postman Repory](https://github.com/Pranayraut23/Phoenix-Inwarranty-Flow/blob/static-content/newman-report.png)

## Project Structure ##
```
Phoenix Inwarranty Flow Collection
├─ Inwarranty-flow Collection.postman_collection.json # Collection file
├─ QA.postman_environment.json # Environment File
└─ testData.csv # TestData File

```
## How to run the project ##
You can run the project on your local system for that :
1. Clone the Project on Local System : https://github.com/Pranayraut23/Phoenix-Inwarranty-Flow.git
2. Install nodeJS and NPM from : https://nodejs.org/en
3. Install Newman using ``` npm install -g newman ```
4. Instal Newman-reporter-htmlextra using ``` npm install -g newman-reporter-htmlextra ```
5. Run the newman commmand :
```
newman run 'Inwarranty-flow Collection.postman_collection.json' \ 
-e QA.postman_environment.json \
-r cli,htmlextra \
--reporter-htmlextra-export ./newman/index.html
```
## HTML Report ##
The report will be created in the newman folder
![Postman Repory](https://github.com/Pranayraut23/Phoenix-Inwarranty-Flow/blob/static-content/newman-report.png)

