# Amazon ECS Service Limits<a name="service_limits"></a>

The following table provides the default service limits, also referred to as quotas, for Amazon ECS for an AWS account which can be changed\. For more information on the service limits for other AWS services that you can use with Amazon ECS, such as Elastic Load Balancing and Auto Scaling, see [AWS Service Limits](https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html) in the *Amazon Web Services General Reference*\.


| Resource | Default Limit | 
| --- | --- | 
|  Number of clusters per Region, per account  |  2000  | 
|  Number of container instances per cluster  |  2000  | 
|  Number of services per cluster  |  1000  | 
|  Number of tasks per service \(the desired count\)  |  1000  | 
|  Number of Elastic Load Balancing target groups per service  |  5  | 
|  Number of tasks using the Fargate launch type, per Region, per account  |  50  | 
|  Number of public IP addresses for tasks using the Fargate launch type, per Region, per account  |  50  | 
|  Number of tasks launched using the Fargate launch type per second, per Region, per account  This limit applies to both standalone tasks and tasks launched as part of a service\.   |  1 sustained, with the ability to burst up to 10  | 
|  Number of tasks launched using the EC2 launch type per second, per Region, per account  This limit applies to both standalone tasks and tasks launched as part of a service\.   |  20 sustained, with the ability to burst up to 100  | 

The following table provides other limitations for Amazon ECS that cannot be changed\.


| Resource | Limit | 
| --- | --- | 
| Number of Classic Load Balancer per service | 1 | 
| Number of tasks launched \(`count`\) per run\-task | 10 | 
| Number of container instances per start\-task | 10 | 
| Number of revisions per task definition family Deregistering a task definition revision does not exclude it from being included in this limit\.  | 1,000,000 | 
| Task definition size limit | 32 KiB | 
| Task definition max containers | 10 | 
| Number of subnets specified in `awsvpcConfiguration` | 16 | 
| Number of security groups specified in `awsvpcConfiguration` | 5 | 
| Maximum size of a shared volume used by multiple containers within a task using the Fargate launch type | 4 GB | 
| Maximum container storage for tasks using the Fargate launch type | 10 GB | 
| Maximum number of tags per resource \(tasks, services, task definitions, clusters, and container instances\) | 50 | 