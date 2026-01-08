# VPC

Created a custom VPC with CIDR 10.0.0.0/16.
This defines the private network for my resources.

#IGW

Internet Gateway connects the VPC to the internet
Required for public internet access.

# Route Table

Route tablet sends all internet traffic to the Internet Gateway.
This makes the subnet public

# Launch EC2 in public subnet

Launched EC2 in public subnet with public IP.
Security group allows SSh access.

# SSH into the instance

1. VPC created -> isolated network
2. Public subnet -> slice of VPC
3. Internet Gateway -> allows internet access
4. Route table updated -> 0.0.0.0/0 ->IGW
5. Security Group allowed SSH from my IP
6. EC2 launched with public IP
7. SSH into EC2 successful -> confirms traffic flow works
