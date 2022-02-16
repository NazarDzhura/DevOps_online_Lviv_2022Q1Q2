# TASK 2.1

**Part 1:**

1. What are the most popular hypervisors for infrastructure virtualization?
The most popular hypervisors are:
	- VMware ESXi/vSphere, 
	- Microsoft Hyper-V,
	- Citrix XenServer,
	- Oracle VirtualBox,
	- Parallels Hypervisor.

2. Briefly describe the main differences of the most popular hypervisors.
	- VMware ESXi/vSphere has numerous software for all types of virtualization: vSphere Client, vSphere software development kits, Storage vMotion, the Distributed Resource Scheduler
	- Microsoft Hyper-V uses MS Windows as a host OS.
	- Citrix XenServer is an opensource, but it has Standard and Enterprise versions.
	- Oracle VirtualBox is also an opensource product, based on Xen. 
	- Parallels Hypervisor primarily was developed for MacOS, now it enables MS Windows, Linux and Google Chrome OS.

**Part 2:**

1.6. Clone an existing VM1 by creating a VM2

![alt text](/m2/task2.1/img/1.6.png "Clone an existing VM1 by creating a VM2")

1.7. Create a group of two VM

![Create a group of two VM](/m2/task2.1/img/1.7.png "Create a group of two VM")

1.8. For VM1, changing its state, take several different snapshots, forming a branched tree of snapshots

![For VM1, changing its state, take several different snapshots, forming a branched tree of snapshots](/m2/task2.1/img/1.8.png "For VM1, changing its state, take several different snapshots, forming a branched tree of snapshots")

1.9. Export VM1. Save the \*.ova file to disk. Import VM from \*.ova file

![Export VM1. Save the \*.ova file to disk. Import VM from \*.ova file](/m2/task2.1/img/1.9.1.png "Export VM1. Save the *.ova file to disk. Import VM from *.ova file")

![Export VM1. Save the \*.ova file to disk. Import VM from \*.ova file](/m2/task2.1/img/1.9.2.png "Export VM1. Save the *.ova file to disk. Import VM from *.ova file")
 
2.2. Configure the USB to connect the USB ports of the host machine to the VM

![Configure the USB to connect the USB ports of the host machine to the VM](/m2/task2.1/img/2.2.png "Configure the USB to connect the USB ports of the host machine to the VM")

2.3. Configure a shared folder to exchange data between the virtual machine and the host

![Configure a shared folder to exchange data between the virtual machine and the host](/m2/task2.1/img/2.3.png "Configure a shared folder to exchange data between the virtual machine and the host")

2.4. Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.

	- NAT:

![Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.](/m2/task2.1/img/2.4.1.png "Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.")

	- Bridged adapter:

![Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.](/m2/task2.1/img/2.4.2.png "Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.")

	- Internal network:

![Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.](/m2/task2.1/img/2.4.3.png "Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.")

	- Host-only adapter:

![Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.](/m2/task2.1/img/2.4.4.png "Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.")

	- Table of connections:

![Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.](/m2/task2.1/img/2.4.5.png "Configure different network modes for VM1, VM2. Check the connection between VM1, VM2, Host, Internet for different network modes. You can use the ping command to do this. Make a table of possible connections.")

3.2. Examine the purpose and execute the basic commands of VBoxManage list, showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm

![Examine the purpose and execute the basic commands of VBoxManage list, showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm](/m2/task2.1/img/3.2.1.png "Examine the purpose and execute the basic commands of VBoxManage list, showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm")

![Examine the purpose and execute the basic commands of VBoxManage list, showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm](/m2/task2.1/img/3.2.2.png "Examine the purpose and execute the basic commands of VBoxManage list, showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm")

**Part 3:**

3.3. Initialize the environment: vagrant init hashicorp/precise64

![Initialize the environment: vagrant init hashicorp/precise64](/m2/task2.1/img/3.3.png "Initialize the environment: vagrant init hashicorp/precise64")

3.4. Run vagrant up and watch for messages during VM boot and startup.

![Run vagrant up and watch for messages during VM boot and startup.](/m2/task2.1/img/3.4.png "Run vagrant up and watch for messages during VM boot and startup.")

3.5, 3.6. Connect to the VM, using SSH. Record the date and time by executing the date command.

![Connect to the VM using the program MobaXterm or PuTTY (can be downloaded from [6]), using SSH. Record the date and time by executing the date command.](/m2/task2.1/img/3.5.png "Connect to the VM using the program MobaXterm or PuTTY (can be downloaded from [6]), using SSH. Record the date and time by executing the date command.")

3.7. Stop and delete the created VM.

![Stop and delete the created VM.](/m2/task2.1/img/3.7.png "Stop and delete the created VM.")