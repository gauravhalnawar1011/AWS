
Auto Scaling
+++++++++++++

-> In realtime we will perform scale up and scale down for LBR based on our requirement

-> Scale up means increasing resources

-> Scale down means decreasing resources

=> Scaling we can do in 2 ways

	1) Verticle Scaling: This involves increasing the power of existing resources.
For example, you might upgrade an instance from 8 GB of RAM to 64 GB of RAM to handle increased workloads.
	2) Horizontal Scaling:This entails increasing the number of machines or servers.
Instead of having just one server, you add more servers to distribute the workload

-> Verticle scaling means increasing the power of existing resources 

		Ex : chaging from 8 GB RAM to 64 GB RAM

-> Horizontal scaling means increasing no.of machines/servers

		Ex : instead of one machine we will take 4 machines



-> In realtime, we will setup Load Balancer for our applications to handle huge traffic

-> When traffic is increasing we need to increases resources to handle that load

-> When traffic is decreasing we need to decrease resources to reduce cost

--------------------------------------------------------------------------------------------
What is Auto Scaling
-------------------------------------------------------------------------------------------

-> We can't predict how many users will access our application in a day

-> If we configure 30 servers to run our application, if traffic is huge then 30 servers may not sufficient. If traffic is less then 30 servers not required

-> Adding & removing servers to Load Balancer is time taking process.

		******* To overcome all the above problems, We have Auto Scaling feature in AWS*******

-> The process of adding/removing servers from load balancer based on the traffic is called as Auto Scaling.


Auto Scaling Advantages
+++++++++++++++++++++++

1) Fault Tolerance: Auto Scaling helps maintain your application's uptime and ensures that even if an instance fails, new ones can be quickly added to replace it.
2) Availability :  It improves your application's availability by dynamically scaling to meet demand, thus reducing the risk of downtime.
3) Cost Management : Auto Scaling enables cost optimization by scaling down during periods of low demand, reducing operational expenses



Steps to setup AutoScaling
++++++++++++++++++++++++++

1) Create Launch Template: This template defines the configuration for the instances that Auto Scaling will launch.

2) Create Auto Scaling Group by selecing Launch Template: You create an Auto Scaling group and associate it with the launch template. This group is responsible for maintaining the desired number of instances based on the specified configurations




