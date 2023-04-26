# Continuous Integration (CI)

- Use CircleCI to operate the Continuous Integration jobs. Connect the Github repo from: https://github.com/khtrieu1102/udacity-aws-deploy to the CircleCI
- Each commit/change to the repo will trigger the pipeline run in CircleCI.

## Pipeline

- CircleCI will read the `.circleci/config.yml` stored in master branch.
- There are total 3 steps in this file: `build`, `hold` and `deploy`.
    * *Build*: will install all dependencies (aws-cli, elastic beanstalk, node, ...) for each project, then trigger the builds (backend and frontend) after `linting`.
    * *Hold*: Need the confirmation of the user in CircleCI to move to the next step `deploy`
    * *Deploy*: Triggers the deploy operations, to publish the FrontEnd Application to S3 Bucket, and the BackEnd Server to the AWS EB.
