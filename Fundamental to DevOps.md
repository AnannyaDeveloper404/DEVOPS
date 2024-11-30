## Fundamental Devops

- It has a culture that improve the organizational ability to delivery the application.
- Automation
- Quality
- Monitoring
- Testing

## Why Devops:

`Development of applications`

- System admin -Creates Server
- Build and release engineer:Deploy application on the server
- server administrator:Create app server

`Delivery to users`

This all responsibilities are tackled by Devops.

## What are the day to day tasks of the Devops engineer:

Roles:

- I take of automation ensuring quality maintained and continuos monitoring and automated the testing process in the devops life cycle;

## Software Development Lifecycle:

- Design |
- Develop|=> High Quality
- Test|

---

`planning+Requirement`->`Defining`->`Designing`->`Building`->`Testing`->`Deploy`->`planning`

- Requirement Gathering :This step is conducted by business analyst ,Strategy team or through a survey to collect feedbacks from customers.
- Defining : Documents (SRS)Software Requirements Specification
- Designing - HLD nd LLD
  - HLD - Scalable when required,n no. of replica
  - LLD- Coding Type,technology
- Automation:These following three are main part of Devops
  - Building
    - Developing=>writing code and pushing to common repository
  - Testing
    - Testing phase (Run on server),Tested by QE(Quality Assurance engineer)
  - Deployment :Promote this to production server

## Virtual Machine (VM)(1)

- What is Server?
- Physical vs Virtual
- Hypervisor
  - Hypervisor is already installed in physical server,and it creates virtual machine.
- How to create vm?

### RealWorld example

- If You request for a vm in AWS of Mumbai branch ,One of the Physical Server's Hypervisor will create a vm for you and will also share you information(Ip address,requested specification like memory,cpu) related to the vm.

## Virtual Machine (VM)(2)

AWS allows for automation.To do this devops engineer writes **script** to make a request to AWS API(EC2,S2) In return it sends ec2 instance.
the request must be valid,authenticated ,authorized.

### Types of **Script**

Means of communicating with aws api

- AWS CLI
- AWS API
- AWS CFT(Cloud formation template)
- AWS CDK(Cloud development Kit)
  - very specific towards aws
- Terraform
- Manual approach (Inefficient ,Time consuming)

### AWS EC2 instance creating

- Log in AWS console
- Service=>EC2
- Go to Instance
- Launch Instances
  ## Same goes for Azure (Manual way to launch instance)
- access EC2 instance in MobaXTerm .

### Logging in the virtual machine manually

- Click on the instance id
- Connect
- You've logged in the vm

#### This process is not recommended

### Recommended

- putty
- iterm(Mac)
- mobaxterm

## Why use linux Operating System:

- Fast
- Open source
- Secure

### Architecture

#### kernel

- Heart of the Operating System
  - Manages system resources like CPU, memory, and I/O devices.
  - process management
  - handling system calls
  - Acts as a bridge between applications and hardware.

### System Libraries

- Abstract raw kernel interactions.
- Provide a simpler, consistent interface for application developers.
- Avoid the need for developers to write complex and error-prone system calls directly..

### Shell command

- cd
- ls
- mkdir
- pwd
- touch <file name>
- cat <file name>
- vi <file name>
- vim <file name>
- ls -ltr
- ls -a
- free -g
- nproc
- df -h
- top
- man <command>

##### shebang

```bash
#!/bin/ksh
```

###### different executable :bin,sh,ksh,dash

#### sh vs bash

- previously both of them were same since sh are forwarded to bash by the linking
- sh are used as dash in ubuntu(It might not work as bash in case of ubuntu)

```bash
#!/bin/ksh
echo "My name is Anannya."
```

to save:

```
esc :wq! -> Enter
```

- execute the bash file command
  ```
  ./<fileName>
  or
  sh  <fileName>
  ```
  if it shows 'permission denied',
