This Module creates  the following resources:

    An S3 bucket with private default acl
    A redshift cluster with IAM role that allows read/write access to the bucket

Input parameters(define these in variables.tf):

    Number of nodes
    Node type/size
    Name of bucket/cluster
    Charge Code tag to be applied to all resources

If you don't provide any inputs it will by default assume following values (you can change this in variables.tf)
    cluster_number_of_nodes = 3
    cluster_port = 5439
    

Outputs(define these in outputs.tf):

    Redshift endpoint
    S3 bucket ARN

Owner: Veerababu
