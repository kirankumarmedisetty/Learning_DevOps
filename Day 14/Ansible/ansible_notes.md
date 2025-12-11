Q. Why Configuration Management came into existence?
Ans: Earlier for eg. upgrading, patching, installations we used to depend on shell/powershell scpting based on servers 
and based on distribution like for eg. Centos, Ubuntu, Debian, Fedora we have to change the scipt. It used to become tedious
task when there are huge number of servers. To overcome this problem Configuration Managment tool like Ansible came into existence.

Q. What are different tools which comes under Configuration Management?
Ans: Ansible, Chef, Puppet and Salt.

*Q. Why ansible is better than other configuration tools like Puppet?
Ans:  Main difference b/t ansible and puppet is as follows. 
Puppet:
1. It uses pull model
2. It followes master and slave agent based architecture
3. It it not that flexible with environments like Windows where we need to strech additionally to 
complete the tasks.
4. We need to learn additonal language which is puppet language.
Ansible:
1. It used push model.
2. It is follows agentless approch.
3. It is very much flexible with both linux/windows where we can find modules for Windows/linux easily 
when compared to Puppet.
4. It uses very simple yaml launguage which is widely used accross globe. 
5. In ansible you can build your own module using python and share it accross different organizations using Ansile Galaxy.

*Q. What is the programming language do you use for building custom modules?
Ans: Ansible uses python as a programming language to build custom modules, . 

*Q. Have you created a customer ansible module using python?
Ans: There was no requirement as of now, but I can write a module whenever it is required.

*Q. Does ansible supports only Windows or only Linux?
Ans: It supports both Windows and Linux. For windows it uses winrm as a protocol to connect and for linux it uses ssh as a protocol.

*Q. Is ansible uses pull or push?
Ans: Ansible is push mechanishm. You run a playbook from a node which connects over ssh/winrm to target nodes and pushes the tasks/configuration immediately. 

*Q. Which language is used for writing playbooks?
Ans: Ansible uses YAML as programming language.

*Q. Does ansible supports AWS/Azure/GCP?
Ans: It supports all the cloud provides. It only require public access and ssh needs port 22 to be opened to connect from host machines where ansible is configured. 

*Q. What is the different b/w ansible adhoc and playbook?
Ans. Using ansible adhoc commands you can execute single commands instently and if you running mutiple tasks on target servers you require playbook for execution. 

*Q. How do you run certain number of tasks on particular servers but not on all servers in a inventory?
Ans. All the servers will be metioned in inventory file and using grouping method I perform certain number of tasks on particular servers. 


