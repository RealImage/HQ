# HQ

### A PaaS controller for AWS that encapsulates best practices

HQ runs on only on your local machine, talking directly to AWS with no intermediate network calls. The source is MIT License and fully auditable. 

Heavily inspired by 

https://github.com/convox/rack

https://github.com/remind101/empire

Both are great options if you want a command line interface, but HQ provides a much simpler, more opinionated model for deploying 12-factor applications, especially Docker containers.

It bakes in the setup of a private network (VPC), a load balancer in a cost effective configuration (ALB + Host Routing), RDS / ElastiCache setup, and application servers on EC2/ECS - setting everything up together with secure default rules. It also helps with easy setup of SNS+SQS linked topics and queues, and S3 buckets with replication.   
