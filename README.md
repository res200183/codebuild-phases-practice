# AWS CodeBuild Phases Practice

This repository demonstrates how AWS CodeBuild executes build phases defined in `buildspec.yml`.

## What is covered
- install phase
- pre_build phase
- build phase
- post_build phase

## Technologies
- AWS CodeBuild
- GitHub
- YAML

## Project goal
The goal of this project is to demonstrate practical understanding of AWS CodeBuild build lifecycle and phase execution order.

## Build phase order
1. install
2. pre_build
3. build
4. post_build

## Files
- `buildspec.yml` — defines the build phases and commands
- `README.md` — project description

## Result
The build runs successfully in AWS CodeBuild and shows the correct phase execution order in logs.

## What I learned
- how AWS CodeBuild uses `buildspec.yml`
- how build phases run sequentially
- how logs reflect each phase execution
- how to connect GitHub as a source provider
