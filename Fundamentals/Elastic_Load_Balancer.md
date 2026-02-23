# ELB-Elastic Load Balncer
<br>
Elastic Load Balancers (ELBs) solve this by acting as a central, intelligent traffic router that distributes requests evenly across healthy servers, detects node failures, and automates scaling, ensuring high availability and seamless performance. <br>

<img width="587" height="336" alt="image" src="https://github.com/user-attachments/assets/7246237d-34aa-407a-baee-d7669c1a8cbb" />


Traffic Distribution: ELB acts as a single point of entry, routing requests to the least busy server to prevent bottlenecks.<br>

Health Checks: ELB continuously monitors the health of instances, automatically stopping traffic to failed instances.<br>

Scalability: ELB works with Auto Scaling to dynamically add or remove instances based on demand.<br>

Session Persistence: It supports "sticky sessions," ensuring a user's requests are sent to the same instance for consistency.<br>

High Availability: ELB can distribute traffic across multiple availability zones. <br>

##  ALGORITHM USED IN ELB-Round-Robin 
<br>
<img width="587" height="336" alt="image" src="https://github.com/user-attachments/assets/bdba5c30-d878-49ac-bc91-7316fab23748" />

<br>
This is a static algorithm that routes incoming requests to targets in a sequential, rotational order. Each healthy target receives an equal share of requests, without considering the current load or number of active connections on each server. This method is simple and commonly used for stateless applications where request processing times are relatively equal across all targets.
