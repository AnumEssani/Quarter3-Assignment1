# Article On Micro services

# What are Micro services?

Micro services are a software development technique —a variant of the service-oriented architecture (SOA) structural style— that arranges an application as a collection of loosely coupled services.
In  a microservices architecture, services are fine-grained and the protocols are lightweight.
Or
In short a microservices architecture is a term used to describe the practice of breaking up an application into a series of smaller, more specialised parts, each of which communicate with one another across common interfaces such as APIs and REST interfaces like HTTP.

# Introduction:
There is no single definition for micro services. A consensus view has evolved over time in the industry. Some of the defining characteristics that are frequently cited include:
Services in a microservice architecture (MSA) are often processes that communicate over a network to fulfill a goal using technology-agnostic protocols such as HTTP.
> •	Services in a microservice architecture are independently deployable.

> •	Services are organized around business capabilities.

> •	Services can be implemented using different programming languages,databases, hardware and software environment, depending on what fits best.

> •	Services are small in size, messaging-enabled, bounded by contexts, autonomously developed, independently deployable, decentralized and built and released with automated processes.

A microservice is not a layer within a monolithic application (example, the web controller, or the backend-for-frontend).Rather it is a self-contained piece of business functionality with clear interfaces, and may, through its own internal components, implement a layered architecture. From a strategy perspective, microservices architecture essentially follows the Unix philosophy of "Do one thing and do it well".

It is common for microservices architectures to be adopted for cloud-native applications,serverless computing, and applications using lightweight container deployment. According to Fowler, because of the large number (when compared to monolithic application implementations) of services, decentralized continuous delivery and DevOps with holistic service monitoring are necessary to effectively develop, maintain, and operate such applications.A consequence of (and rationale for) following this approach is that the individual microservices can be individually scaled. In the monolithic approach, an application supporting three functions would have to be scaled in its entirety even if only one of these functions had a resource constraint. With microservices, only the microservice supporting the function with resource constraints needs to be scaled out, thus providing resource and cost optimization benefits.


# Background:
	
During the early days of Software Development, barriers to entry in Programming languages were high and only people with PhD in Science and Mathematics could use those programming languages. In 1964, a general-purpose programming language BASIC was developed. It lowers the barrier so that non-PhD students from all departments can also write programs. As there was a rapid growth of computing applications in the 1960s, software became large and complex. Computer Scientists tried to tackle the complexity of Software Systems with the ancient and proven technique: Divide and Conquer.

David Parnas published his seminal paper “On the Criteria to be used in decomposing Systems into Modules” in 1972 which introduced the concepts of Modularityand Information hiding. Also,Edsger W. Dijkstra introduced the concept Separation of Concern in his paper “On the role of scientific thought” published in 1974. The works of Parnas, Dijkstra and others lead to the rise of Modular Software Development in the 1970s with the principal of decomposing a large, complex software system into “Loosely coupled, highly cohesive” modules which communicated via internal interfaces. In simple terms, “loosely coupled” means the dependency between modules should be very low and “highly cohesive” means that one module should focus on single or similar functionality. With the rise of the Internet and Web in the 1990s, software systems became widespread in business applications and became even more complex and large. Although Modularity is used to reduce the complexities of software application, it often did not help as the soft Modular boundaries of software sub-systems are easy to cross and misuse. Another Software Architecture pattern became very popular during the 1990s to develop business applications:Layered Architecture. Normally, a business Web Application is divided into several layers: Presentation, Business, Database layers.

# Monolithic Architecture:

Structures an application as a single executable and deployable component. Monolithic architecture is actually a good choice in building simple applications, but there is an architecture that is better for large and complex systems which will be covered in a moment. Some of the benefits of building a monolithic-based application are as follows:
> •	Simple to develop

> •	Easy to make radical changes

> •	Easy to scale

> •	Straightforward to test and deploy

Since a monolithic-based application is a single component, we deliver, deploy, and test it easily in a straightforward manner. Once an application gets larger and even more complex, we face the following challenges [1]:
> •	Complexity

> •	Slow development

> •	Commit to deployment

> •	Difficulty in scaling

> •	Reliability

> •	Obsolete

A large and complex monolithic-based application slows down the IDE of the developer which leads to development and deployment issues. This type of application may experience difficulty in adopting new features and new technology. To address these challenges, Microservice Architecture is developed and introduced to the industry.

# Microservice Architecture:
In the 2010s, other disruptive technologies arise which impact the Software Development landscape in a significant way:Cloud Computing, Containerization (Docker,Kubernetes),DevOps. Likewise some highly productive, lightweight new programming languages e.g. Golang, Rust, Swift come to the scenario whereas some highly productive, easy to use, lightweight programming language like JavaScript, Python become mainstream. There is a change in Software Development model also. Waterfall software development model is almost discarded and replaced by fast, iterative, incremental Software development methodology:Agile Software development. Computer Hardware also changed massively with cheaper, faster main memory and rise of Multi-Core CPU, GPU. There was a change in the Data Storage landscape as well. New Database technologies like NoSQL, NewSQL emerges and become mainstream.
To handle the complexity of modern software applications, to take the advantages of Cloud Computing, Containerization, DevOps, modern Programming languages and to fulfill the need of modern software development (fast development, horizontal scaling), a new Software Architecture Style arose in 2012: Microservice Architecture. So, what is exactly a Microservice Architecture? There are many definitions of Microservice Architecture and here is my definition:
“Microservice Architecture is about decomposing a Software System into autonomus Units which are independently deployable and which communicates via lightweight, language agnostic way and together they fulfill the business goal.”
Microservice Architecture also uses the same technique of divide and conquer to tackle the complexity of software systems like Modular Monolithic architecture where a complex Software system is divided into many Microservices which communicates via external Interfaces. The key difference between Modular Monolithic and Microservice Architecture is that every Microservice can be deployed independently whereas all Modules usually are deployed as a whole (deployment Monolith).
Monolithic application is one single unit (tightly coupled) like a single Cube. Modular application is like Rubric Cube which can contain small modules but the modules cannot be separated and can only be deployed together. Microservices are like a lego cube made by lego blocks where the blocks are loosely coupled, easily separable and all the lego blocks together made the cube.
