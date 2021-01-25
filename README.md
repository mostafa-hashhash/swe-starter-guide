# Software Engineering Starter Guide
to collect all the important topics that need to be covered in one place, and clarify how all these topics are connected together in a meaningful way

# Table of Contents
[1. Languages & Runtime Environments](#1-languages--runtime-environments)  
[2. Networking & Communication Protocols](#2-networking--communication-protocols)  
[3. Operating System Concepts](#3-operating-system-concepts)  
[4. Database Management Systems](#4-database-management-systems)  
[References](#references)

Building a strong enough foundational knowledge helps greatly in **understanding** the different technologies in-depth and how they are working behind the scenes, in addition to gaining the ability to **build new** solutions and tools


# 1. Languages & Runtime Environments

**Core Concepts** ⇒  Data types, functions, conditional statements, loops, arrays, Memory Allocation & Execution Stack 

**Common libraries for using** ⇒ Input/output, files, algorithms and data structures, mathematical operations 

**Compilation process** ⇒ Stackoverflow [Discussion](https://stackoverflow.com/questions/6264249/how-does-the-compilation-linking-process-work) , Compilation [process](https://www.javatpoint.com/compilation-process-in-c) in C

**Errors** ⇒ Logical, Syntax, Compilation, Runtime

**Building Process** ⇒ Compilation & Interpretation

**Code Files Types** ⇒ Source code, Machine code, Byte code, Object code

**Programming Paradigms** ⇒ Imperative, Declarative, Functional, Object-oriented

**Typing** ⇒ Static & Dynamic

**Object-Oriented Paradigm** 

- **Concepts** ⇒ Class, Object, Abstraction, Encapsulation, Inheritance, Base Class, Interface
- **Design Principles** ⇒ [SOLID](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design) , [Refactoring](http://sourcemaking.com/refactoring/smells)

---

# 2. Networking & Communication Protocols

It's very important to know how each is communicating with the rest and why we use the specific choices, so for sure you need to understand the connectivity of the internet, and the accessibility of each component of your system so we will discuss what is the Virtual Private Network ( VPC ), Addressing with IPs and Subnets, and for development purposes, we will dig deep in the most popular protocols of the web.

the idea of the protocol is to have some common rules for our communication, how we will process the messages to understand and perform operations, so there're many protocols to cover all communication stuff, database queries, web content, emails, files, getting the corresponding IP of the domain, remote access, exchanging the routing information, exchanging encryption, sending the network error messages, routing in the network, ... etc.

### 2.1 Networking Fundamentals

**Basic Terminologies** ⇒  Routers, LAN, WAN, Gateway, Subnets, IP, Port __ Articles: [1st](https://implictthoughts.wordpress.com/2019/05/18/walk-through-computer-networking-fundamentals-part-1/), [2nd](https://implictthoughts.wordpress.com/2019/05/19/walk-through-computer-networking-fundamentals-part-2/), [3rd](https://implictthoughts.wordpress.com/2019/05/20/walk-through-computer-networking-fundamentals-part-3/) __ [Information Technology Playlist](https://www.youtube.com/playlist?list=PL7zRJGi6nMRzHkyXpGZJg3KfRSCrF15Jg) 

### 2.2 Reference Models Layers

The main purpose of these steps will be to provide interoperability between the systems, which means to have standard rules for information exchanging to understand it. ____ Roadmap Channel [video](https://www.youtube.com/watch?v=dV8mjZd1OtU&ab_channel=theroadmap) ___ Hussien Nasser channel [video](https://www.youtube.com/watch?v=7IS7gigunyI&ab_channel=HusseinNasser)

### 2.3 Protocols in Each Layer

**1. Application Layer Protocols ( HTTP, WS )**

- **HTTP (Hypertext Transfer Protocol)**
URL Anatomy [Explanation](https://www.youtube.com/watch?v=ADQ_rhefgEk) & Difference Between Query string and URL Parameters

    Basic [Concepts](https://www.youtube.com/watch?v=RsQ1tFLwldY) of Web Application ,, [How](https://www.youtube.com/watch?v=hJHvdBlSxug&ab_channel=Academind) The Web Works ,, Request/Response [Structure](https://www.youtube.com/watch?v=sxiRFwQ1RJ4)

    HTTP Generations [Talk](https://www.youtube.com/watch?v=idViw4anA6E&ab_channel=Codegram) - HTTP ,, Another [one](https://youtu.be/0OrmKCB0UrQ) from Hussien Nasser

    Head-of-line-blocking in TCP and HTTP/1.1

    HTTP2 ⇒ has **Multiplexing** instead of ordered and blocking, **Server Push** to add responses proactively to reduce the number of requests

    HTTP/2 Critical [Limitation](https://www.youtube.com/watch?v=GriONb4EfPY&ab_channel=HusseinNasser) that led to HTTP/3 & QUIC

- **DNS (Domain Name System)** ⇒ Roadmap Channel [Explanation](https://www.youtube.com/watch?v=Wj0od2ag5sk)
- **SSH (Secure Shell)** for remote access
- **Web Sockets** ⇒ Hussien Nasser [Video](https://youtu.be/2Nt-ZrNP22A) ,, SSE vs WebSockets vs Long Polling [Talk](https://www.youtube.com/watch?v=n9mRjkQg3VE&ab_channel=FestGroup)
- **Message Queue Protocols ( e.g MQTT, AMQP )**

**2. Transport Layer protocols** 

- **TCP & UDP** ⇒ Roadmap [video](https://www.youtube.com/watch?v=37AFBZv4_6Y) | HusseinNasse [video](https://www.youtube.com/watch?v=qqRYkcta6IE)  |  [Applications](https://www.youtube.com/watch?v=G86axGfnWag) Use Cases

**3. Network Layer Protocols**

- **[ARP](https://www.youtube.com/watch?v=mqWEWye-8m8&ab_channel=HusseinNasser) ( Address Resolution Protocol ) __ [NAT](https://www.youtube.com/watch?v=RG97rvw1eUo&ab_channel=HusseinNasser) ( Network Address Translation )** **&** **PAT (** **Protocol Address Translation )**

---

# 3. Operating System Concepts

Where do you think all our systems live & operate? Anything running on the computer uses its resources from CPU cycles, memory, network, or disk operation. So there should be some layer between these H.W. resources and their consumers

**Basic Terminologies**

- Processes, Threads, Context Switching, Scheduling, System API Calls [ I/O, DB, … ] | CPU Cores & Threads
- Caching & Pagination, Resources Allocation, Sockets, Kernel & H.W, Init Process | Virtual Machines | Concurrency Vs. Parallelism

**Resources**

- Cracking The Coding Interview ( Chapter 15 ) __ Programming Interviews Exposed ( Concurrency Chapter )
- Operating System Internals And Design Principles __ The little book of semaphores __ Medium [Article](https://medium.com/cracking-the-data-science-interview/the-10-operating-system-concepts-software-developers-need-to-remember-480d0734d710)
- Understanding Embedded Linux [Playlist](https://www.youtube.com/playlist?list=PLWXRxAK4bUzc9gq-W2xWDe9zEaDcowLfs) __ The 10 OS Concepts SWD Need to Remember - [Article](https://medium.com/cracking-the-data-science-interview/the-10-operating-system-concepts-software-developers-need-to-remember-480d0734d710)

**Processes**

[Virtual Memory](https://www.youtube.com/watch?v=hEh6ZVP_U1w) ( During The Execution ) ,, [State Diagram](https://www.youtube.com/watch?v=JhWREa77Z88) ( The Life Cycle )

**Shell Process & Terminal** as an interface to execute the binaries through **Commands** and **Environment Variables**

Executing Commands in The Shell as a Processes  ⇒  [Part_1](https://www.youtube.com/watch?v=lrQpf39CbFA)  |   [Part_2](https://www.youtube.com/watch?v=3QTDkcnlH9A)  |  [Part_3](https://www.youtube.com/watch?v=cli9fyCvbWQ)

There's a huge relationship between the O.S. and the system files. Actually, Linux is Handling anything through files, the media devices like USB, Storage devices, Processes, Users, Libraries, everything is a file so we can access the O.S. stuff with some paths in the [file Systems](https://www.youtube.com/watch?v=KN8YgJnShPM)

Now, you know the commands, the shell process, the processes, and the signals. So imagine every application is a process and the OS may receive signals from a user to change the process state, so we can make a script ( some shell commands ) or an application ( like the system monitor ) or a package ( like PM2 ) to manage the processes life cycle. In case of any failure, we can kill a poisoned process or restart the production application, in addition to collecting some information about all the processes in different states for monitoring.

---

# 4. Database Management Systems

Data is everywhere, think of your online messages, profiles, sensors data, media, or whatever. So It's important to design some **rules** for easy storing, retrieving, processing it for any reason like analysis and providing recommendations. So the **Database systems** were designed for that purpose, simply by initializing a **process** to **communicate** ( sending the queries and receiving the records, or information about the transaction state ) with other services through a **port**. 

The server spins up a connection pool to make multiple requests to the database instance at the same time. And to communicate with the DB we need a library on the server-side to interface between the server and the DB instance and provide some security features 

**Resources**

Relational  [Article](https://dev.to/lmolivera/everything-you-need-to-know-about-relational-databases-3ejl) & Non Relational ( NOSQL ) [Article](https://dev.to/lmolivera/everything-you-need-to-know-about-nosql-databases-3o3h) ___ 7 Database Paradigms [video](https://www.youtube.com/watch?v=W2Z7fbCLSTw)

Cracking The Coding Interview ( Chapter 14 ) & HackerRank Database Questions

**Transaction Consistency Models** ⇒ ACID, BASE

**Distributing the database instances**

- **Partitioning** ⇒ Horizontally (Sharding) or Vertically ( with different schema )
- Clustering trade-offs ( Advantages & Problems of them )
- Different **Replication** paradigms ⇒ Leader-follower or Mesh ( point-to-point communication using gossip )
- **Configuration management** tools like ZooKeeper
- **PACELC** Theorem for distributed systems

for Relational DB ⇒ Practice on

- Querying multiple tables with **Joins**
- **Pagination** to get a sequential subset of the records with an OFFSET and LIMIT or WHERE to make it [faster](https://www.youtube.com/watch?v=WDJRRNCGIRs&ab_channel=HusseinNasser)

**Views & Materialized Views** to cache some hot results instead of re-search for them continuously 

**MVCC ( MultiVersion Concurrency Control** **)** as implied in the name enables us to allow concurrent access to a database.

**Buffer Pool** which is the DB area in the RAM used for caching or any intermediate operation before hitting the disk storage 

**Transactions & Locks for Race Conditions**

---
# References

**Technical** 

- [MozilaDocs](http://developer.mozilla.org) ,, [GoogleDocs](http://developers.google.com/web)
- Conferences ⇒ QConf, InfoQ, Devoxx, GOTO Conferences, KubeCon, DockerCon, PyConf, JSConf
- Technical Blogs from Big Tech Companies
- Technical Articles from developers e.g [Medium.com](http://medium.com) , [Dev.to](http://dev.to)

**Presentation Diagrams** ⇒ [Gliffy](https://gliffy.com) ,, [Draw](https://draw.io)

**Downloading Books** ⇒ [http://library.lol/](http://library.lol/) ,, PDF drive

**Searching for Jobs** ⇒ Glassdoor, Crossover, Linkedin, Microverse, CarrerArch, Toptal, Remoteplatz
