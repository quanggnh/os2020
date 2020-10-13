### Lec 09 Runtime architecture

#### 1 What is the purpose of the Describe the Run-time Architecture activity?

To analyze concurrency requirements, to identify processes, identify inter-process communication mechanisms, allocate inter-process coordination resources, identify process lifecycles, and distribute model elements among processes.

#### 2 What is a process?  What is a thread?

- Process
  + Provides heavyweight flow of control
  + Is stand-alone
  + Can be divided into individual threads
- Thread
  + Provides lightweight flow of control
  + Runs in the context of an enclosing process

#### 3 Describe some of the considerations when identifying processes.

- Utilize multiple CPUs and/or nodes
- Increase CPU utilization
- Service time-related events
- Prioritize activities
- Achieve scalability (load sharing)
- Separate the concerns among software areas
- Improvement of system availability
- Support major subsystems

### Lec 10 Distribution

#### 1 What is the purpose of the Describe Distribution activity?

To describe how the functionality of the system is distributed across physical nodes. Required only for distributed systems.

#### 2 What is a node?  Describe the two different “types” of nodes.

- Node
  + Physical run-time computational resource
  + Processor node
    + Executes system software
  + Device node
    + Support device
    + Typically controlled by a processor

#### 3 Describe some of the considerations when mapping processes to nodes.

- Distribution patterns
- Response time and system throughput
- Minimization of cross-network traffic
- Node capacity
- Communication medium bandwidth
- Availability of hardware and communication links
- Rerouting requirements
