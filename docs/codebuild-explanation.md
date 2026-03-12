# AWS CodeBuild Build Phases

AWS CodeBuild uses a file called `buildspec.yml` to define the build process.

## Build phase order

CodeBuild executes phases in the following order:

1. install
2. pre_build
3. build
4. post_build

## Phase explanation

### install
Used to prepare the build environment.

Typical tasks:
- install dependencies
- install runtime
- configure tools

### pre_build
Preparation before the main build.

Typical tasks:
- authentication (ECR login)
- retrieving secrets
- preparing environment variables

### build
The main build phase.

Typical tasks:
- compiling code
- running tests
- building Docker images

### post_build
Executed after a successful build.

Typical tasks:
- pushing Docker images
- uploading artifacts
- sending notifications

## Key concept

All phases run inside the same build container, so files and environment variables remain available between phases.
