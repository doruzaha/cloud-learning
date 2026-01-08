# Day 8 Notes

## VPC

A VPC is a logically isolated virtual network in AWS. 
It defines IP ranges, routing, and security boundaries.
All AWS resources run inside a VPC.

## CIDR blocks

CIDR deines the size of a network.
Smaller number = larger network.
AWS VPCs use private IP ranges.

## Subnets

Subnets divide a VPC into smaller networks.
Each subnet belongs to one AZ ( availability zone).
Public and private subnets control access.

## Public vs Private subnets

Public subnets have internet access.
Pivate subnets do not.
Databases should be in private subnets.

## Internet Gateway

Internet Gateway connects a VPC to the internet.
Required for public subnets.

## Route Tables

Route tablets control traffic flow.
0.0.0.0/0 means all internet traffic.
Public subnets route to an Internet Gateway

## Security Groups (VIRTUAL FIREWALL)

Security Groups act as instance-level firewalls.
They allow traffic, not deny.
They are stateful.

## Full trafic flow

Traffic flow depends on VPC, subnet, routes, and security groups.
All components must be correctly configured.
