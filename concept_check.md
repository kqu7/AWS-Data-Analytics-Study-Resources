## Introduction
This section contains selected concepts/features I encountered while doing practice problems on some third-party platforms such as Whizlab. This is not a comprehensive listing, but you can probably use it for self-check.

## Table of Contents
- [Amazon S3](#Amazon-S3)
- [Amazon Kinesis Streams](#Amazon-Kinesis-Streams)
- [Amazon Kinesis Firehose](#Amazon-Kinesis-Firehose)
- [Amazon Kinesis Analytics](#Amazon-Kinesis-Analytics)
- [Amazon EC2](#Amazon-EC2)
- [Amazon DynamoDB](#Amazon-DynamoDB)
- [Amazon Redshift](#Amazon-Redshift)
- [Amazon Glue](#Amazon-Glue)
- [Amazon EMR](#Amazon-EMR)
- [Amazon Athena](#Amazon-Athena)
- [Amazon DMS](#Amazon-DMS)
- [Amazon ElasticSearch](#Amazon-ElasticSearch)
- [Others](#Others)

<div style="text-align: right"> ⬆️  &nbsp; <a href="./README.md">Back to the Main Page</a> </div>


**Note:** 
- for each service or feature, should at least think about *how it works* and its *use cases*

## Amazon S3
### Additional Features
- [Amazon S3 inventory](https://docs.aws.amazon.com/AmazonS3/latest/userguide/storage-inventory.html)

- [Logging requests using server access logging](https://docs.aws.amazon.com/AmazonS3/latest/userguide/ServerLogs.html)

### Security Concern
- [Access policy guidelines](https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-policy-alternatives-guidelines.html)

## Amazon Kinesis Streams
### Architecture: 
- Sources
    - [Kinesis Agent](https://docs.aws.amazon.com/streams/latest/dev/writing-with-agents.html#pre-processing)


### Performance Concern
- [Handling Duplicate Records](https://docs.aws.amazon.com/streams/latest/dev/kinesis-record-processor-duplicates.html)


- [Troubleshooting Kinesis Data Streams Consumers](https://docs.aws.amazon.com/streams/latest/dev/troubleshooting-consumers.html)

- [A deep-dive into lessons learned using Amazon Kinesis Streams at scale](https://acloudguru.com/blog/engineering/deep-dive-into-aws-kinesis-at-scale)


- [Troubleshooting Kinesis Data Streams Consumers](https://docs.aws.amazon.com/streams/latest/dev/troubleshooting-consumers.html)
    - [Common issues, questions, and troubl shooting ideas for consumers](https://docs.aws.amazon.com/streams/latest/dev/troubleshooting-consumers.html#misc-troubleshooting-consumer)


## Amazon Kinesis Firehose
### Additional Features
- [Amazon Kinesis Data Firehose Data Transformation](https://docs.aws.amazon.com/firehose/latest/dev/data-transformation.html) 

## Amazon Kinesis Analytics
---
## Additional Features
- [Schema Discovery](https://docs.aws.amazon.com/kinesisanalytics/latest/dev/sch-dis.html)

## Amazon Elastic Compute Cloud (EC2)
---
### Architecture
- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html) 
    - [Snapshot](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html)
    - [Performance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSPerformance.html)
    - [Encryption](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html)

## Amazon DynamoDB
### Architecture
- [Core Components of Amazon DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.CoreComponents.html)

- [Read/Write Capacity Mode](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadWriteCapacityMode.html)

- [DynamoDB Backups](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Backups.html)

### Additional Features
- [Amazon DynamoDB Accelarator](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DAX.html)

- [How to use Amazon DynamoDB global tables to power multiregion architectures](https://aws.amazon.com/blogs/database/how-to-use-amazon-dynamodb-global-tables-to-power-multiregion-architectures/)

- [DynamoDB Streams Use Cases and Design Patterns](https://aws.amazon.com/blogs/database/dynamodb-streams-use-cases-and-design-patterns/)

### Performance Concern
- [My DynamoDB table is being throttled](https://aws.amazon.com/premiumsupport/knowledge-center/dynamodb-table-throttled/)

- [How do I choose the right primary key for a DynamoDB table?](https://aws.amazon.com/premiumsupport/knowledge-center/primary-key-dynamodb-table/)

## Amazon Redshift
### Architecture
- [Data distribution style](https://docs.aws.amazon.com/redshift/latest/dg/c_choosing_dist_sort.html)
- [Working with Sort Keys](https://docs.aws.amazon.com/redshift/latest/dg/t_Sorting_data.html)
- [Redshift Sort Key - Choosing Best Sort Key](https://hevodata.com/blog/redshift-sort-keys-choosing-best-sort-style/)

### Additional Features:
- [Using COPY to load data](https://docs.aws.amazon.com/redshift/latest/dg/t_Loading_tables_with_the_COPY_command.html)
    - [Loading data from Amazon EMR](https://docs.aws.amazon.com/redshift/latest/dg/loading-data-from-emr.html)
    - [Loading data from remote hosts](https://docs.aws.amazon.com/redshift/latest/dg/loading-data-from-remote-hosts.html)

- [Vacuuming tables](https://docs.aws.amazon.com/redshift/latest/dg/t_Reclaiming_storage_space202.html#vacuum-types)

- [AQUA (Advanced Query Accelerator)](https://docs.aws.amazon.com/redshift/latest/mgmt/managing-cluster-aqua.html)

- [Implementing automatic WLM](https://docs.aws.amazon.com/redshift/latest/dg/automatic-wlm.html)

- [Working with concurrency scaling](https://docs.aws.amazon.com/redshift/latest/dg/concurrency-scaling.html)

- [Working with short query acceleration](https://docs.aws.amazon.com/redshift/latest/dg/wlm-short-query-acceleration.html)

- [Working with recommendations from Amazon Redshift Advisor](https://docs.aws.amazon.com/redshift/latest/dg/advisor.html)

- [Creating a temporary staging table](https://docs.aws.amazon.com/redshift/latest/dg/merge-create-staging-table.html)
    - [Use a staging table to perform a merge (upsert)](https://docs.aws.amazon.com/redshift/latest/dg/c_best-practices-upsert.html)

### Integration with Other Services:

- [Kinesis Adapter](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.KCLAdapter.html)

- [Working with Kinesis Data Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/kds.html)

- [Working with DynamoDB Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/kds.html)


### Performance Concern:
- [Overview of managing clusters in Amazon Redshift](https://docs.aws.amazon.com/redshift/latest/mgmt/managing-cluster-operations.html#elastic-resize)
    - Elastic Resize
    - Classic Resize

- [ETL and ELT design patterns for lake house architecture using Amazon Redshift: Part 1](https://aws.amazon.com/blogs/big-data/etl-and-elt-design-patterns-for-lake-house-architecture-using-amazon-redshift-part-1/)

- [ETL and ELT design patterns for lake house architecture using Amazon Redshift: Part 2](https://aws.amazon.com/blogs/big-data/etl-and-elt-design-patterns-for-lake-house-architecture-using-amazon-redshift-part-2/)

- [Amazon Redshift Advisor recommendations](https://docs.aws.amazon.com/redshift/latest/dg/advisor-recommendations.html#enable-sqa-recommendation)



## Amazon Glue
### Additional Features
- [Overview of Workflows in AWS Glue](https://docs.aws.amazon.com/glue/latest/dg/workflows_overview.html)

- [How can I use AWS Glue workflows to automatically start a job when a crawler run completes?](https://aws.amazon.com/premiumsupport/knowledge-center/start-glue-job-after-crawler-workflow/)

- [AWS Glue Triggers](https://docs.aws.amazon.com/glue/latest/dg/about-triggers.html)

## Amazon Elastic MapReduce (EMR)
### Configuration
- [Create a cluster with instance fleets or uniform instance groups
](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-instance-group-configuration.html)

### Additional Features:
- [Integrate with AWS Lake Formation](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-lf-conceptual.html)
- [Call Amazon EMR with Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/connect-emr.html)

- [Introducing Amazon EMR Managed Scaling – Automatically Resize Clusters to Lower Cost](https://aws.amazon.com/blogs/big-data/introducing-amazon-emr-managed-scaling-automatically-resize-clusters-to-lower-cost/)

### Security Concern
- [Amazon VPC options](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-clusters-in-a-vpc.html)

- [Encryption options](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-data-encryption-options.html)

- [Secure your data on Amazon EMR using native EBS and per bucket S3 encryption options](https://aws.amazon.com/blogs/big-data/secure-your-data-on-amazon-emr-using-native-ebs-and-per-bucket-s3-encryption-options/)

## Amazon Athena
### Architecture
- Data Sources
    - [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/data-sources-glue.html) 
    - [Hive Metastore](https://docs.aws.amazon.com/athena/latest/ug/connect-to-data-source-hive.html)
    - [Athena Federated Query](https://docs.aws.amazon.com/athena/latest/ug/connect-to-a-data-source.html)

### Additional Features:
- [Workgroup](https://docs.aws.amazon.com/athena/latest/ug/user-created-workgroups.html)
- [Separate queries and managing costs using Amazon Athena workgroups](https://aws.amazon.com/cn/blogs/big-data/separating-queries-and-managing-costs-using-amazon-athena-workgroups/)

### Security Concern:
- [Data Protection in Athena](https://docs.aws.amazon.com/athena/latest/ug/security-data-protection.html)

- [Fine-Grained Access to Databases and Tables in the AWS Glue Data Catalog](https://docs.aws.amazon.com/athena/latest/ug/fine-grained-access-to-glue-resources.html)

## Amazon Data Migration Service (DMS)
### Architecture
- [How AWS Database Migration Service works](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Introduction.html)
- [Heterogeneous database migration](https://docs.aws.amazon.com/prescriptive-guidance/latest/migration-oracle-database/heterogenous-migration.html)

### Performance Concern: 
- [How can I troubleshoot high target latency on an AWS DMS task?](https://aws.amazon.com/premiumsupport/knowledge-center/dms-high-target-latency/)

## Amazon ElasticSearch
### Additional Features: 
- [Kibana](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-kibana.html)
- [Using Kibana with Amazon Elasticsearch Service](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-kibana.html#es-kibana-proxy)

## Others
[Amazon SNS](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)
- [Using Amazon SNS for application-to-application (A2A) messaging](https://docs.aws.amazon.com/sns/latest/dg/sns-system-to-system-messaging.html)

[AWS IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
- [Role concepts](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_terms-and-concepts.html)
- [Managed policies and inline policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_managed-vs-inline.html)

[AWS Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html)
- [User pool](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-identity-pools.html)
    - [Adding Sign-in Through a Third Party](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-identity-federation.html)

- [Identity pool](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-identity.html)
    - [Identity pool concepts](https://docs.aws.amazon.com/cognito/latest/developerguide/concepts.html)
- [Amazon Cognito Streams](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-streams.html)


[AWS VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- [NAT gateways](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html)

[AWS CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/WhatIsCloudWatchEvents.html)


[AWS Secrete Manager](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html)


[AWS Kinesis Video Stream](https://docs.aws.amazon.com/kinesisvideostreams/latest/dg/what-is-kinesis-video.html)

[Amazon Macie](https://docs.aws.amazon.com/macie/latest/user/what-is-macie.html)


[Amazon Neptune](https://docs.aws.amazon.com/neptune/latest/userguide/intro.html)


[Amazon ElasticCache](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/WhatIs.html)
- [Common ElastiCache Use Cases and How ElastiCache Can Help](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/elasticache-use-cases.html)
- [Comparing Memcached and Redis](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/SelectEngine.html)
