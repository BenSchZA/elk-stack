## Deployment

`eb init elk --profile __profilename__ -p "64bit Amazon Linux 2018.03 v2.10.0 running Multi-container Docker 17.12.1-ce (Generic)"`

`eb create elk-service`

`eb deploy`

Open incomming port 5601 of EC2 instance.

## Elastic Beanstalk

Current working directory where files are located /var/app/current/ 

## Local

For ElasticSearch:

sudo sysctl -w vm.max_map_count=262144

To make this permanent:

sudo echo 'vm.max_map_count=262144' >> /etc/sysctl.conf

After this either restart server or use sysctl command to set.
