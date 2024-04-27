# Assignment - 6
##  Write an ansible-playbook to install nginx on target servers.

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404


### 1) What is YAML
YAML, short for "YAML Ain't Markup Language," is a human-readable data serialization format. It's often used for configuration files, data exchange between programs, and as a language-independent way to represent structured data.
**Key features:**

*Readability:* YAML files are designed to be easily readable by humans. It uses indentation to denote structure, similar to Python.

*Structure:* YAML represents data using key-value pairs, lists, and nested structures. It supports arrays, dictionaries, and scalar values like strings, integers, and booleans.

*Comments:* YAML supports comments, making it convenient for annotating configurations and data.

*Data Types:* YAML supports various data types, including strings, integers, floats, booleans, arrays, objects, and null values.

*Platform Independence:* YAML is designed to be language-independent, making it easy to use across different programming languages and platforms.

### 2) What is Ansible
Ansible is an open-source automation tool used for configuration management, application deployment, and task automation. It simplifies the process of managing and orchestrating infrastructure by allowing users to describe their infrastructure in simple, human-readable YAML files called "playbooks."

*Agentless:* Unlike some other configuration management tools, Ansible is agentless, meaning it doesn't require agents to be installed on managed hosts. Instead, it uses SSH (Secure Shell) and Python to communicate with remote servers.

*Inventory:* Ansible uses an inventory file to define the hosts it will manage. This inventory can be static or dynamic, allowing for flexible management of infrastructure.

*Playbooks:* Playbooks are written in YAML and contain a series of tasks that define the desired state of the system. Tasks can include actions such as installing packages, copying files, starting services, and running commands.

*Modules:* Ansible provides a wide range of built-in modules that can be used within playbooks to perform various tasks on managed hosts. These modules abstract common system administration tasks and make it easy to automate complex workflows.

*Idempotent:* Ansible playbooks are idempotent, meaning they can be run multiple times without causing unintended side effects. If a task has already been completed and the system is in the desired state, Ansible will skip it during subsequent runs.

*Roles:* Ansible roles are a way to organize and package playbooks, allowing for better code reuse and maintainability. Roles encapsulate reusable components, making it easier to manage complex configurations across multiple systems.

### Write a ansible-playbook to install nginx on servers.

-  Create 4 EC2 instances
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/15dbcf18-5182-4f96-b665-36d599aacd65)

-   Connect to ansible master and run the following commands:
```
sudo yum install ansible
```

-   Generate a ssh key on Ansible-master using command and copy it.
```
ssh-keygen
```

-   Do the same on ansible server1 and copy the key.

-   Login to ansible master and try ssh connection.

-   Create a dir in master, ansible-project and create inventory text file and write ip of each asnible server.
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/77f080cc-d0d0-4443-a7d2-3c1ffb35d810)

-   Create a playbook, first-playbook.yml and write the code.
```
-	name: Install and restart the nginx
hosts: all
become: true
tasks:
  -	name: install nginx
    apt: name=nginx state=latest
  -	name: start nginx
    service:
      name: nginx
      state: started

```
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/cd1e6fcf-2103-467d-88e5-cdf3b4d35934)

-   Execute the play book using command:
```
ansible-playbook -i inventory first-playbook.yml
```

-   Check on each server if nginx is installed.
