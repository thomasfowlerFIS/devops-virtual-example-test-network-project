# **VETNet Project Guidelines**

## **Learning Goals**

* Build a virtual network using multiple virtual machines that communicate
with one another.

* Configure a virtual machine to act as a network router between other
routers on the virtual network.

--------------------------------------------

### **Overview**

Build a virtual network using multiple virtual machines where each Node on
the network can communicate with one another via a virtual Router.

* Utilize the concepts in the previous lessons in virtualization to configure
a virtual network.

* Investigate various methods to provide network communication
between the nodes on the virtual network.

The instructions below will guide you through the process of planning
the virtual network. Take into consideration the requirements outlined
below and use the minimum amount of software and configuration
necessary to satisfy the project requirements.

> **_Note_**: It is expected that every dependency needed to implement the
> solution is explained in detail in a document as to its necessity
> and how it is used. When submitting a solution, it is expected this
> accompanying document is included in the submission.

--------------------------------------------

### **Requirements**

For this project, you must:

* Create 6 separate virtual machines from a single virtual machine.

* Configure 3 of the 6 virtual machines to act as nodes on the network
which sit behind their own unique router. In other words, each node on
the virtual network has exactly one router to which it connects.

* Configure 3 of the 6 virtual machines to act as routers to allow
for communication between the nodes.

* When securely connecting to each node, `traceroute` must be succesfully
perormed to every other node. For example, Node 1 must be able to
successfully `traceroute` to Node 2 and Node 3; Node 2 must be able to
successfully `traceroute` to Node 1 and Node 3, and so on.

* Nodes **must not** be able to communicate with the Host, but the Host
must be able to communicate with the Nodes and Routers on the virtual
network.

See the figure below:

<img src="https://raw.githubusercontent.com/thomasfowlerFIS/devops-virtual-example-test-network-project/master/assets/VETNet_Diagram.png" width="600" /> 

--------------------------------------------

### **Project Guidance**

* Use NAT and internal network virtual networking modes to establish connectivity between Routers and Nodes.

* Research software packages and dependencies to enable network
communication across the various components of the virtual network.

* Make sure to establish the correct CIDR rules and network masking for
Routers especially.

--------------------------------------------

### **Resources**

* [VirtualBox Documentation](https://www.virtualbox.org/manual/UserManual.html)
