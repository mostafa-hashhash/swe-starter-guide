# Software Engineering Starter Guide
to collect all the important topics that need to be covered in one place, and clarify how all these topics are connected together in a meaningful way

# Table of Contents
1. [Example](#example)
2. [Example2](#example2)
3. [Third Example](#third-example)
4. [Fourth Example](#fourth-examplehttpwwwfourthexamplecom)


## Example
## Example2
## Third Example
## [Fourth Example](http://www.fourthexample.com) 

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
