1) install the terraform and setup the path
2) install the aws cli and configure the keys 
profile for the aws cli : your user home directory .aws config /credintials
we are going to create the vpc using the terraform
provider: aws
region :
resource: vpc
cidr: 10.1.0.0/16
enable dns = true

subnets
pubsubnets = ["10.1.0.0/24","10.1.1.0/24",10.1.2.0/24"]
anable public ip
privatesubnets = ["10.1.3.0/24",10.1.4.0/24",10.1.4.0/24"]
datasubnets = ["10.1.6.0/24",10.1.7.0/24",10.1.8.0"]
 
 igw
 attach =

 eip=
 nat = pubsubnet[0]

 route table
 pubroute
 privateroute

 associate the pubsubnets with the igw in the public route
 associate the private with the nat-gw in the private route
