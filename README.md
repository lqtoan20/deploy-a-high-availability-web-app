# deploy-a-high-availability-web-app

Project Setup
Files included:
stacks: inclue all cloudfomation template

- network.yaml - CloudFormation network infrastructure stack description.
- network-parameters.json - Parameters file for the network infrastructure stack
- servers.yaml - CloudFormation services infrastructure stack description
- servers-parameters.json - Parameters file for the services infrastructure stack

script: help to run create, delete, update CloudFormation stack easy

- create.sh
- delete.sh
- update.sh

1. To create networking resources using cloudformation template, run the below command.
   $ scripts/create.sh network-stack stacks/network.yml stacks/network-params.json

2. To create servers resources using cloudformation template run the below command.
   $ scripts/create.sh server-stack stacks/servers.yml stacks/servers-params.json
