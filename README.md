# case-study
Creates a stack that will handle leads from dynamo db, sends it on sqs via lambda and will be consumed by another lambda which will insert in a crm.Failure with send SMS in my phone and retry the process twice, Success will send it to other sqs.


**The cloudformation template/stack is caseStudy.yaml**


The folder case-study-via-sceptre is also an option and it contains the cloudformation stack inside as a template and can be used to provision cfn stacks.

How to run via sceptre
1. Install python virtual environment then activate it
2. run this to install sceptre : pip install sceptre-v2
3. cd to case-study-via-sceptre
4. run this code : sceptre create dev/caseStudy.yaml -y


Note: make sure that .aws/credentials and .aws/config are already setup
