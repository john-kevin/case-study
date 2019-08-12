# case-study
 Creates a stack that will handle leads from dynamo db, sends it on sqs via lambda and will be consumed by another lambda which will insert in a crm.Failure with send SMS in my phone and retry the process twice, Success will send it to other sqs
