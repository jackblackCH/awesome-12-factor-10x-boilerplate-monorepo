awesome-12-factor-10x-multi-purpose-clean-code-app-boilerplates-monorepo
========================================================================

First Draft.

## What
- A monorepo containing a super minimal default setup, following 12-factor-app principles for each software stack in this repository.
- Each stack contains all basics and preconfigured configs and files
- Same default setup with modern core principles for each stack. 
- "Plug and Play".
- Stacks are running together but independently
  - Communication only via exposed interfaces
- Supports multiple stacks/languages/frameworks 
  - PRs are welcome

## Why
It is tedious and time consuming to setup and connect the basics for a modern software stack following all core principles of modern software engineering
It's generaly not difficult, but needs a lot of time (and knowledge of the given landscape in the stack). 
Let's start with it, instead of "do it later".

## For whom?
- Lazy but strict developers who follow "clean code" and 12-factor-app principles
- Developers who don't want to reinvent the wheel and stick to common standards
- TDD and XP driver devs
- zero config devs
- DevOps

## How
- Use what you need. 
- Delete what you don't. 
- Don't worry about anything. It just works.

It acts as a plug and play boilerplate for a multi-purpose (at the moment: web) software stack including all features and tools to enforce modern and proven principles of modern software design and engineering.   

## Core Principles
All stacks MUST follow and contain the principles of

- Component based
- Flat
- Supports deployment to a cloud provider
  - Google Cloud
  - AWS
- Docker (preconfigured)
- DevOps
- Infrastructure as Code (preconfigured)
- TDD (examples)
- CI/CD (preconfigured)

### Acceptance criteria of this repo
- A `docker-compose up` must run this all included stacks at once, independently!
- Not needed stacks can be deleted, no config files need to be touched.
- Each stack must contain:
  - README.md file explaining the decissions.
  - Best practice and simple file architecture
  - Best practice configured test library/environment
  - Best practice package/dependency management (i.e npm, composer, gradle)
  - Preconfigured deployment configuration to
    - AWS
    - Google Cloud
  
## Example drafts of stacks (more to be defined and added by the community)

- java (TBD)
- java-whatever (TBD)
- node-express (TBD)
- node-aws-lambdas (TBD)
  - package.json
  - components
- php-vanilla (TBD)
- php-lavarel (TBD)
  - vendor
  - tests
  - components
  - TBD
- python (TBD)
  - requirements.txt
  - components
  - tbd
  - TBD
- web-angular (TBD)
  - TBD
- web-next-app (TBD)
  - package.json
  - tests
  - components
  - api
    - demo.js
- web-react (TBD)
  - package.json
  - tests
  - components
    - button
      - styles.js
      - index.js
      - test.js
  - TBD
- mobile-react-native (TBD)

... open for contributions
- lerna.json (maintaining this repo and components)
- package.json
- docker-compose.yml (runs all the stacks that are in the repository)
- test.js (meta tests for this repo and configs to work. ensure the project runs correctly)
- README.md (explains this repo)

## Resources
All thoughts and patterns are mainly based on the following principles
- 12-factor-app: https://12factor.net/
- CleanCode: https://www.amazon.de/gp/product/0132350882/
