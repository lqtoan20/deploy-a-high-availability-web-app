# deploy-a-high-availability-web-app

Files included:
+ diagram: structure of project
+ stacks: inclue all cloudfomation template

- network.yaml - CloudFormation network infrastructure stack description.
- network-parameters.json - Parameters file for the network infrastructure stack
- servers.yaml - CloudFormation services infrastructure stack description
- servers-parameters.json - Parameters file for the services infrastructure stack

+ script: help to run create, delete, update CloudFormation stack easy

- create.sh
- delete.sh
- update.sh

+ Project Setup

1. To create networking resources using cloudformation template, run the below command.
- $ scripts/create.sh network-stack stacks/network.yml stacks/network-params.json

2. To create servers resources using cloudformation template run the below command.
- $ scripts/create.sh server-stack stacks/servers.yml stacks/servers-params.json

URL test: http://serve-webap-4r7tptwvf0je-1242999771.us-east-1.elb.amazonaws.com/
