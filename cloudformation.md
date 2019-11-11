# CloudFormation

## General

- **[CloudFormation Coverage Roadmap ](https://github.com/aws-cloudformation/aws-cloudformation-coverage-roadmap/projects/1)**: This is a public roadmap focused on upcoming coverage support for CloudFormation. It is focused on coverage additions to existing AWS services to be addressed by upcoming CloudFormation releases.

## Tooling and Libraries

#### Patterns and Examples

- **[widdix/aws-cf-templates](https://github.com/widdix/aws-cf-templates)**: A fantastic repository of reusable templates for CloudFormation by widdix.
- **[stelligent/cloudformation_templates](https://github.com/stelligent/cloudformation_templates)**: This repository contains a collaboration of general and specific Amazon Web Services CloudFormation Template Examples by Stelligent.
- **[awslabs/aws-cloudformation-templates](https://github.com/awslabs/aws-cloudformation-templates/)**: A collection of useful CloudFormation templates by AWS.


#### Generation

- **[AWS CDK](https://github.com/aws/aws-cdk)**: Software development framework to define cloud infrastructure in code and provision it through AWS CloudFormation. The CDK is available JavaScript, TypeScript, Python, Java amd .NET Core.
- **[troposphere]()**: The troposphere library allows for easier creation of CloudFormation by writing Python code to describe the AWS resources. 
- **[cfn-skeleton](https://github.com/awslabs/aws-cloudformation-template-builder)**: A command line tool and Go library that consumes the published CloudFormation specification and generates skeleton CloudFormation templates with mandatory and optional parameters of chosen resource types pre-filled with placeholder values.

#### Serverless

- **[AWS SAM](https://github.com/awslabs/serverless-application-model)**: The AWS Serverless Application Model (SAM) is an open-source framework for building serverless applications. It provides shorthand syntax to express functions, APIs, databases, and event source mappings. It simplifies the CloudFormation that would normanlly be required to create such resources.

#### Custom Resources

- **[crhelper](https://github.com/aws-cloudformation/custom-resource-helper)**: A Python library to simplify best practice Custom Resource creation, sending responses to CloudFormation and providing exception, timeout trapping, and detailed configurable logging.

#### Management and Orchestration

- **[ansible](https://docs.ansible.com/ansible/latest/modules/cloudformation_module.html)**: The ansible module for CloudFormation that launches or updates a stack and waits for it complete. Combine this with other tasks to create a powerful Ansible playbook to orchestrate deployments.
- **[stacker](https://github.com/cloudtools/stacker)**: A tool and library used to create & update multiple CloudFormation stacks.
- **[sceptre](https://github.com/Sceptre/sceptre)**: Sceptre manages the creation, update and deletion of stacks while providing meta commands which allow users to retrieve information about their stacks.
- **[rain]()**: Rain is a development workflow tool for working with AWS CloudFormation.

#### Formatting

- **[cfn_flip](https://github.com/awslabs/aws-cfn-template-flip)**: Converts AWS CloudFormation templates between JSON and YAML formats, making use of the YAML format's short function syntax where possible.
- **[cfn-format](https://github.com/awslabs/aws-cloudformation-template-formatter)**: Reads in an existing AWS CloudFormation template and outputs a cleanly-formatted, easy-to-read copy of the same template adhering to standards as used in AWS documentation.

#### Linting

- **[cfn-nag](https://github.com/stelligent/cfn_nag)**: Looks for patterns in CloudFormation templates that may indicate insecure infrastructure.
- **[cfn-lint](https://github.com/aws-cloudformation/cfn-python-lint)**: Validate CloudFormation yaml/json templates against the CloudFormation spec and additional checks.

#### Validation

- **[taskcat](https://github.com/aws-quickstart/taskcat)**: Tests AWS CloudFormation templates. It deploys your AWS CloudFormation template in multiple AWS Regions and generates a report with a pass/fail grade for each region.

- **[CloudFormation Checklist](https://cfnchecklist.com/)**: A UI Checklist to generate a report on the maturity of a teams CloudFormation development, deployment and management to enforce best practices.

## Workshops and Tutorials

- **[AWS Cloudformation Advanced (Reinvent 2018)](https://github.com/aws-samples/aws-cloudformation-advanced-reinvent-2018)**: Learn how to use AWS CloudFormation custom resources, mappings and constraints, StackSets, and macros to increase your infrastructure automation efficiency, while simultaneously addressing complex business requirements.
