# Pipeline Process

The pipeline is connected with my GitHub account with this repository as project in CircleCI.
It follows the steps in .circleci folder

## Order of Pipeline Steps

1. The pipeline uses orbs to install Node, the AWS cli and the EB cli.
2. It clones out the code from the repo
3. Install Depedencies for Frontend & API
4. Builds Frontend & API
5. Deploys Frontend using AWS CLI S3 to copy files to the Bucket, And AWS CLI EB to deploy nodejs API to eb environment.