## VPC (Virtual Private Cloud) - A Guide

### Introduction to VPC

- VPC (Virtual Private Cloud) is a fundamental service in AWS used to create virtual networks.
- It allows you to set up your private network in the AWS cloud environment.

### VPC in AWS

- In AWS, you create Virtual Machines using three main services: EC2, EBS, and VPC.
- VPC is considered a "Customer Managed Service," as opposed to AWS Managed Services (SaaS).
- VPC is essential for launching virtual machines in AWS.

- # VPC: Virtual Private Cloud

## Introduction
- We create Virtual Machines in AWS to set up our infrastructure.
- The main AWS services for creating virtual machines are:
  1. EC2 (Elastic Compute Cloud)
  2. EBS (Elastic Block Storage)
  3. VPC (Virtual Private Cloud)
- VPC is a customer-managed service in AWS and is a critical part of creating and managing your network infrastructure.

## IP Addressing
- When creating a VPC, you specify an IP address range, known as the CIDR block, for the VPC.
- IP ranges in IPV4 are divided into classes, and CIDR (Classless Inter-Domain Routing) notation is used to define IP ranges.
- Common private IP address ranges used in VPCs:
  1. 10.0.0.0/16
  2. 172.16.0.0/12
  3. 192.168.0.0/16

## Subnets
- Subnets are used to divide the IP address range of a VPC into smaller, more manageable segments.
- Subnets can be public or private, depending on whether they have internet access.

## Internet Gateway
- An Internet Gateway (IGW) is used to allow instances in your VPC to connect to the internet.

## Route Tables
- Route tables are used to control the traffic between subnets within your VPC.
- Route tables are associated with subnets and determine where network traffic is directed.

## NAT Gateways
- Network Address Translation (NAT) gateways allow instances in private subnets to initiate outbound traffic to the internet while preventing unsolicited inbound traffic.

## Security Groups and NACL
- Security Groups and Network Access Control Lists (NACLs) are used for controlling inbound and outbound traffic to and from your instances.

## VPC Flow Logs
- VPC Flow Logs can be enabled to track incoming and outgoing traffic in your VPC.

# VPC Peering
- VPC Peering allows the routing of traffic between different VPCs.

## VPC Peering Setup
- To establish VPC peering, you need two VPCs with non-overlapping CIDR blocks.
- You must create a peering connection and configure route tables in both VPCs to allow traffic to flow.

# Custom VPC Creation
- You can create custom VPCs, specifying the IP address range, subnets, and other networking components.

# Note
- Always remember to clean up resources to avoid unnecessary costs.

---

# Additional Information (Optional)
- You can customize your VPC to fit your organization's needs.
- Choose private IP address ranges carefully to avoid IP conflicts.


### Understanding VPC with an Analogy

Think of VPC as a 2 BHK flat:

- Land with a main gate is like entering your VPC.
- Inside the house, there are rooms (Subnets) with separate doors (networks).
- Some rooms have public access (Public Subnets), while others are private (Private Subnets).
- Public Subnets are rooms accessible from the street, while private subnets are rooms hidden from public view.
- To provide security, we configure security rules using Security Groups and NACL (Network Access Control List).

### VPC Elements

Key components of a VPC:

- VPC
- Subnets (Public and Private)
- Internet Gateway (Ingress and Egress)
- Route Table (Connections to Subnets)
- NAT Gateways (Outgoing traffic)

### Internet Gateway vs. NAT Gateway

- Internet Gateway (IGW) allows both incoming and outgoing traffic.
- NAT Gateway only supports outgoing traffic, providing a level of security.

### Security in VPC

- Security is maintained in VPC through Security Groups and Network Access Control Lists (NACL).
- Security Groups work at the resource level, while NACLs work at the subnet level.
- Security Groups allow traffic to be "allowed," while NACLs provide the option for both "allow" and "deny."

### Monitoring with VPC Flow Logs

- VPC Flow Logs track incoming and outgoing traffic in your VPC.
- They help you keep records of who is accessing your resources.

### IP Addressing and CIDR Blocks

- IP address ranges in VPC are calculated using CIDR (Classless Inter-Domain Routing).
- Understand IPv4 and IPv6 address formats and the concept of CIDR.
- Plan your IP allocation carefully to avoid running out of IP addresses.

### Lab Task: Setting Up VPC

1. Create a Custom VPC (e.g., "ashokit_custom_vpc") with your chosen CIDR range.

2. Create Subnets in the VPC, both public and private.

3. Create EC2 instances in the subnets.

4. Set up an Internet Gateway to allow traffic for the EC2 instances in public subnets.

5. Create Route Tables and associate them with the respective subnets.

6. Establish VPC Peering between the default VPC and the custom VPC.

7. Modify the Route Tables for VPC Peering to enable communication.

8. Ensure proper security group configurations for both VPCs.

9. Test connectivity between instances from different VPCs.

## VPC Peering: Enabling Communication Between VPCs

### What is VPC Peering?

- VPC Peering is a feature that allows traffic to flow between two Virtual Private Clouds (VPCs).
- It enables communication between EC2 instances in different VPCs as if they were on the same network.

### When to Use VPC Peering

VPC Peering is useful when:

- You want to connect resources across different VPCs, like connecting development and production environments.
- You need to establish communication between VPCs owned by different accounts.
- You want to share resources and data between VPCs securely.

### Steps to Set Up VPC Peering

1. **Create the VPCs:**

   You need at least two VPCs that you want to connect. One will act as the requester, and the other as the accepter.

2. **Create Peering Connection:**

   - In the AWS Management Console, navigate to VPC -> Peering Connections.
   - Create a new peering connection and specify the requesting and accepting VPCs.
   - Send a peering connection request to the accepter VPC.

3. **Accept Peering Connection:**

   - In the accepter VPC, navigate to VPC -> Peering Connections.
   - Accept the connection request from the requester VPC.

4. **Update Route Tables:**

   - In both VPCs, update the route tables to include routes for the peered VPC.
   - This allows traffic to be routed correctly between the VPCs.

5. **Security Groups and NACLs:**

   Ensure that the security groups and Network Access Control Lists (NACLs) allow the desired traffic between the instances in the peered VPCs.

6. **Test Connectivity:**

   Verify that you can establish connections between instances in the peered VPCs using private IP addresses.

### Limitations of VPC Peering

- VPC Peering is not transitive. If VPC A is peered with VPC B and VPC C, VPC B and VPC C are not peered with each other.
- Overlapping IP address ranges are not allowed between peered VPCs.
- Each peering connection is limited to a specific VPC. To establish multiple peering connections, you must create separate connections for each VPC pairing.

### Cost of VPC Peering

- VPC Peering itself is generally free. You are charged for the data transfer between the peered VPCs.

### AWS VPC Sizing

- When designing a VPC, it's crucial to plan the IP addressing carefully.
- IP addressing is divided into classes. In AWS, the concept of CIDR (Classless Inter-Domain Routing) is used to allocate IP addresses.

#### Understanding CIDR

- In IPv4, addresses are divided into classes A, B, C, D, and E. Class E is reserved for experimental purposes.
- CIDR notation specifies the number of significant bits in an IP address.
- For example, a CIDR block like `10.0.0.0/16` means that the first 16 bits are the network address, and the remaining bits are host addresses.
- You can choose a range that best fits your VPC size, but it should not overlap with other VPCs or conflict with reserved IP ranges.
- AWS recommends using a /16 CIDR block (65,536 IP addresses) for VPCs.

#### Default VPC

- Each AWS region comes with a default VPC, which can be used for launching instances easily.
- However, for more control and security, it's better to create a custom VPC.
- The custom VPC allows you to specify your own IP range and configure your subnets, route tables, and other networking components.

#### VPC Peering

- VPC peering is a feature that allows the connection of two VPCs.
- Traffic between peered VPCs remains within the AWS network, without going over the internet.
- CIDR ranges must not overlap between the VPCs, and you must create route entries to enable communication.

### Conclusion

Understanding VPCs, CIDR notation, and how to properly size and manage IP address ranges is essential when designing your AWS infrastructure. Custom VPCs offer greater control, security, and customization for your cloud resources.

## References

- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/index.html)
- [VPC Peering Documentation](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html)
- [CIDR Notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing)
