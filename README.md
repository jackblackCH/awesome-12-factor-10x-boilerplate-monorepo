12-factor-10x-fullstack-hybrid-app-boilerplate-monorep
======================================================

First Draft.

# What?
- A monorepo containing a super minimal default setup for each software stack in this repository. 
- Each stack contains all basics and preconfigured configs and files
  - (PRs following the principles are welcome)
- Same default setup with core modern core principles for each stack. 
- "Plug and Play".
- Stacks are running independently 
  - Communication only via exposed interfaces
- Supports multiple stacks/languages/frameworks 
  - PRs are welcome

# Why
It is tedious and time consuming to setup and connect the basics for a modern software stack following the core principles.
It's generaly not difficult, but needs a lot of time. 
Let's start with it, instead of "do it later".

# How
- Use what you need. 
- Delete what you don't. 
- Don't worry about anything. It just works.

It acts as a plug and play boilerplate for a multipurpose web software stack including all features and tools needed to enforce modern and proofed princriples of modern (web) software design.   

## Core Principles

All stacks MUST follow the principles of

- Infrastucture as Code
- Componented based
- Flat
- Support a Cloud Provider
  - Google
  - AWS
- Docker
- DevOps
- Cloud Infrastructure
- Infrastructure as Code
- CI/CD
- Extreme Programming

### Ressources
All thoughts and patters are mainly based on the following principles
- 12-factor-app: https://12factor.net/
- CleanCode: https://www.amazon.de/gp/product/0132350882/

### Acceptance criterias of a stack
- A `docker-compose up` must run this whole repository with all containing stacks 
- Not needed stacks can be deleted, no config files need to be touched.
- Each stack must contain
  - A command runner
  - Package / Dependency management system (i.e npm, composer, maven)
  - A working tests enviroment,
  - A working deployment command to a preconfigured dev and prod env to a cloud provider (aws, google)

## Mainainted Stacks

- stacks
  - node 
    - components
    - TBD
  - php (TBD)
    - tests
    - components
    - TBD
  - react (
    - tests
    - components
    - TBD
  - python (TBD)
    - components
    - tbd
    - TBD
  - ... open for contributions
    
- docker-compose.yml (runs all the stacks that are in the repository)
- test.js (meta tests for the plug and play setup. ensure the project runs correctly)
- README.md
