# AWS: Cloud Servers
Amazon Web Services provides a highly reliable, scalable, low-cost infrastructure platform in the cloud that powers hundreds of thousands of businesses in 190 countries around the world. With data center locations in the U.S., Europe, Brazil, Singapore, Japan, and Australia, customers across all industries are taking advantage of the following benefits:

1. Low Cost
2. Agility and Instant Elasticity
3. Open and Flexible
4. Secure

## AWS EC2

Its Secure and resizable compute capacity for virtually any workload

And offers the broadest and deepest compute platform, with over 500 instances and choice of the latest processor, storage, networking, operating system, and purchase model to help you best match the needs of your workload.

## EC2 For Humans

EC2 is one of the most important services AWS offers. and how to create inestance of AWS and configure it so we can use it, then we should add storage, add tags, configure security group, and review instanse launch, this is the step to connect to AWS.

AWS is a comprehensive, evolving cloud computing platform; EC2 is a service that enables business subscribers to run application programs in the computing environment. It can serve as a practically unlimited set of virtual machines (VMs).

## Elastic Beanstalk

It's an easy to use service that manages web apps and services, and will automatically scale your applications And it help you to market faster.

# Virtual Machine
In computing, a virtual machine (VM) is the virtualization/emulation of a computer system. Virtual machines are based on computer architectures and provide functionality of a physical computer. Their implementations may involve specialized hardware, software, or a combination.

Types of virtualization Therefore, software and hardware manufacturers have begun to address some of these concerns by shifting how traditional data centers are architected via virtualization. There are the various types of virtualization:

- Hardware virtualization: Virtualizing hardware, including versions of computers and operating systems (VMs), creates a single, virtual, consolidated, primary server.

- Software virtualization: Creates a computer system, including hardware, that allows one or more guest OS to run on a physical host machine.

- Storage virtualization: Virtualizes storage by consolidating multiple physical storage devices, which appear as a single storage unit for improved performance and increased speed.

- Network virtualization: Enables application-driven cloud virtual networking across an entirely distributed set of systems, decoupling from physical network infrastructure. Network virtualization allocates bandwidth across channels, providing resources to servers and devices in real-time.

- Desktop virtualization: Separates your desktop environment from the physical device and stores a desktop on a remote server, allowing access from anywhere on any device.

**Containers vs. virtual machines** Containers and virtual machines are both used by developers and IT professionals to create isolated virtual environments for testing and developing software. Whereas a virtual machine depends on a host to run a complete operating system, a container is an isolated silo that runs an application on the host. Containers run applications that are not dependent on an operating system—rather, they isolate an application by virtualizing it.

Since containers don’t contain operating systems, containers are lightweight and more portable than virtual machines. And even though containers are portable, they’re still constrained by their operating system; so that a container for Windows is unable to run on Linux. In the end, deciding between a container or a virtual machine depends on how a virtual environment will be used.

**What are VMs used for?** Here are a few ways virtual machines are used:

- Building and deploying apps to the cloud.
- Trying out a new operating system (OS), including beta releases.
- Spinning up a new environment to make it simpler and quicker for developers to run dev-test scenarios.
- Backing up your existing OS.
- Accessing virus-infected data or running an old application by installing an older OS.
- Running software or apps on operating systems that they weren't originally intended for.

**What are the benefits of using VMs?**

Because of their flexibility and portability, virtual machines provide many benefits, such as:

- Cost savings— running multiple virtual environments from one piece of infrastructure means that you can drastically reduce your physical infrastructure footprint. This boosts your bottom line—decreasing the need to maintain nearly as many servers and saving on maintenance costs and electricity.
- Agility and speed— Spinning up a VM is relatively easy and quick and is much simpler than provisioning an entire new environment for your developers. Virtualization makes the process of running dev-test scenarios a lot quicker.
- Lowered downtime— VMs are so portable and easy to move from one hypervisor to another on a different machine—this means that they are a great solution for backup, in the event the host goes down unexpectedly.
- Scalability— VMs allow you to more easily scale your apps by adding more physical or virtual servers to distribute the workload across multiple VMs. As a result you can increase the availability and performance of your apps.
- Security benefits— Because virtual machines run in multiple operating systems, using a guest operating system on a VM allows you to run apps of questionable security and protects your host operating system. VMs also allow for better security forensics, and are often used to safely study computer viruses, isolating the viruses to avoid risking their host computer.