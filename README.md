# Project 2 - CI/CD

#### Application background
Application code was downloaded from @edeediong timezone_checker repo. This application is used to tell the user the time in another timezone using the cmd. 

#### Workflow used - publish.yml
1. Publish python distributions to TestPyPI when there is a push/pull to master
Steps:
a. Build a job that runs on ubuntu
b. Checkout the project and set up py env
c. Install dependencies and test code against a linter
d. Create source distribution
e. Upload the contents to TestPyPI - note that API token from TestPyPI is required and use it create a secret in the repo
