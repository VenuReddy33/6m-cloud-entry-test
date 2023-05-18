# Cloud Infrastructure Engineering - (6 Months) Entry Assessment

## Objective

This assessment aims to test your resourcefulness, the ability to understand IT concepts, and produce a viable answer to the problems listed.

---
## Submission

- Create an account in github.com
- Fork this repository to your account
- Use the online editor to edit this file (README.MD)
- Save your changes
- Submit the URL of this repository 
- Ensure your URL is publicly accessible

---
## Expected Audience

- Individuals with an IT background to diversify/expand their skills and/or intending to switch to a software developer role.
    - Those with IT or Engineering degree/diploma, or
    - Those with IT or Engineering experience professionally
- Individuals with systems and infrastructure administration background.
- Individuals who have attended basic infrastructure or cloud courses.

---

## Problems

Please attempt the solve the problems described:

**Question 1 - IP Address**

What is the Bash command to discover the IP Address of `www.skillsunion.com`?

```sh
# ping www.skillsunion.com
```

---

**Question 2 - Copy a Directory**

What is the command to copy a directory from `~/my_project` to `/etc/projects`?

```sh
# cp -r ~/my_project /etc/projects


**Note: It is assumed that my_project is the source directory to copied here. If the source directory is a sub directory in my_project, the command would be cp -r ~/my_project/src_dir /etc/projects where src_dir is the source directory

```
---

**Question 3 - Shell Scripting**

Implement a bash script that does the follow:
1. Convert a string "one,two,three" into an array delimited by comma (,).
1. Loop through the array and print each element.

```sh
# IFS=',' read  -a arr <<< "one,two,three"
# for i in "${arr[@]}"; do echo $i; done
```

---

**Question 4 - System Architecture Diagram**

Use [draw.io](draw.io) to draw a system architecture diagram as described below:

- A load balancer to manage request between 4 application servers.
- The load balancer is connected to the internet gateway.
- All application servers are connected to a cluster of database.
- The cluster of database contains an instance for reading and another instance for writing.
- The database must not be connected to the internet gateway.

Share the link to your image of diagram.

https://drive.google.com/drive/folders/1x1w9gvrWlrjfRlKHmjwb6ixhEtMHSyFZ?usp=share_link


---

**Question 5 - System Error Management**

Alan has deployed his web application to Amazon Web Service. Unfortunately, the web application encountered errors as complained by the customers (public users). Whenever there is a complaint, Alan would take a long time to trace the issue and get back to the customers. 

*Q5A: Which of the following described the scenario given?*

A - The principle of security is not applied.

B - The principle of observability is not applied.

C - The principle of availability is not applied.

D - The principle of performance is not applied.

*Q5B: What do you suggest could be done to improve the situation?*

```
A5A: C - The principle of availability is not applied.

A5B: To improve the situation, The geo redundancy of the application can enhanced by deploying the web application in multiple availability zones of AWS. Alan could also explore using multiple EC2 instances or implement auto scaling of EC2 and making use of Elastic load balancer to distribute the traffic.


```

---

END
