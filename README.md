# Jenkins jobs task

- This Jenkins job can be triggered via `curl` command, which will clone the project (details-app) from https://github.com/orinahum/Details_App.git and build container with it and push that container to docker hub registry
- The Freestyle configuration is copied into "Jenkins_Job_Copy" for review.
### Steps
- Triggered by curl: localhost/job/Docker_Build_Push/build?token=build
- The freestyle job in jenkins will run, and will perform the next steps: 
    - Clone project(details-app) from https://github.com/orinahum/Details_App.git
    - Build docker images
    - Tag docker images with docker hub registry to push to.
    - Push to registry https://hub.docker.com/r/alayani/details_app

