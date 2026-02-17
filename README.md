# System Design

System Design is the process of designing the architecture, components, and interfaces for a system so that it meets the end-user requirements. 

## Importance of System Design

System design is important for anyone who wants to build a robust, scalable, and efficient software application. 

* **Scalability and Reliability:** Ensures systems can grow without failure.
* **Efficient Resource Management:** Optimizes resource allocation.
* **Adaptability:** Allows systems to evolve with business needs.

## Core Components

### HLD (High Level Design)
**Initial step** in the development of applications where the overall structure of a system is planned.



# Monolithic Architecture - System Design
Monolithic architecture is a software design methodology that combines all of an application's components into a single, inseparable unit. Under this architecture, the user interface, business logic, and data access layers are all created, put into use, and maintained as one, unified unit.

A traditional approach in system design, which contains all application components into a single codebase.
It was preferred for its simplicity and ease of initial setup.
In contrast, alternative architectural approaches, like microservices, divide the application into smaller, separately deployable services.
Because of its rigidity, it is difficult to scale and maintain, which makes it difficult to adjust to changing needs.

<img width="225" height="225" alt="image" src="https://github.com/user-attachments/assets/440a7bb7-0058-47fe-aa74-d059ceb8511b" />

## Importance of Monolithic Systems
Single Codebase: All components are developed and maintained in one codebase, simplifying management.






## What is server?
<br>
-> Where we host our site or deploy our projects.
<br>
-> Server has its own IP Address
<br>

## DNS <img width="40" height="35" alt="image" src="https://github.com/user-attachments/assets/2fdf0dd8-c47b-460d-8ea7-62d8486600e6" />


-> The Domain Name System (DNS) is often referred to as the "phonebook of the Internet". 
<br>
-> It is a hierarchical, distributed database that translates human-readable domain names (e.g., www.google.com) into numerical IP addresses (e.g., 192.0.2.1) that computers use to identify each other on the network. 
<br>
-> Allows humans to use memorable names to access websites instead of memorizing complex numeric IP addresses.
<br>

# Server Down Problem
<br>
-> A "server down" problem occurs when a website or online service becomes inaccessible, slow, or completely non-functional. In technical terms, it means the server—the computer storing the website's data—is not responding to user requests. 
<br>
-> When a website goes down, visitors might see errors like "503 Service Unavailable," "Database Connection Error," or a simple "Site Cannot Be Reached" message. 
<br>
<br>
## The "Result Day" Scenario: An Example of Server Overload
<br>
Imagine a popular Board Exam (like CBSE) is releasing results for 1 million students at 12:00 PM.
<br>
Limited Resources (The "Store" Capacity): The education board’s website operates on a set of servers (hardware) with limited processing power (CPU), memory (RAM), and network capacity. 
This is like a small corner shop designed to serve 100 people a day.<br>

Lot of User Requests (The "Rush"): At 12:00 PM, 500,000 students, parents, and teachers try to log in simultaneously.

<br>Millions of requests hit the database to retrieve individual results.<br>

The Crash (The "Congestion"): The server tries to handle all requests at once.

<br>It runs out of RAM and CPU power, slowing down to a halt or shutting down to prevent damage.<br>

Result: The website crashes. Students see error screens or just a loading wheel. 

<br>It is, as one expert described, "like forcing a stadium's crowd through a single exit". <br>


So , in this we can do that either go for <br>

1-Horizontal Scaling <br>
2-Vertical Scaling

<img width="587" height="336" alt="image" src="https://github.com/user-attachments/assets/4e4c6f90-0abd-4c75-b887-7e86728d07cf" />


Horizontal Scaling<br>

Horizontal scaling (scaling out) increases system capacity by adding more machines to a network, offering high, near-limitless scalability, better fault tolerance, and no downtime. 

Vertical scaling <br>

Vertical scaling (scaling up) upgrades an existing server's resources—CPU, RAM, or storage—providing simpler management but limited capacity and potential downtime. 

##  Problem in Horizontal Scaling <br>

Complexity & Management: Managing multiple instances increases operational overhead, making monitoring and orchestration more difficult than a single, large machine.<br>

Data Consistency & Synchronization: Ensuring all nodes have identical, updated data is difficult. Without proper replication, this leads to data corruption or conflicting information.<br>


## How to resolve this:-<br>

# ELB-Elastic Load Balncer
<br>
Elastic Load Balancers (ELBs) solve this by acting as a central, intelligent traffic router that distributes requests evenly across healthy servers, detects node failures, and automates scaling, ensuring high availability and seamless performance. <br>



















