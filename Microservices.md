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

# Benefits of Microservices:
The benefit of decomposing an application into different smaller services are numerous:
> •	Modularity: This makes the application easier to understand, develop, test, and become more resilient to architecture erosion. This benefit is often argued in comparison to the complexity of monolithic architectures.


> •	Scalability: Since microservices are implemented and deployed independently of each other, i.e. they run within independent processes, they can be monitored and scaled independently.

> •	Integration of heterogeneous and legacy systems: microservices is considered as a viable mean for modernizing existing monolithic software application.There are experience reports of several companies who have successfully replaced (parts of) their existing software by microservices, or are in the process of doing so.The process for Software modernization of legacy applications is done using an incremental approach.

> •	Distributed development: it parallelizes development by enabling small autonomous teams to develop, deploy and scale their respective services independently. It also allows the architecture of an individual service to emerge through continuous refactoring. Microservice-based architectures facilitate continuous integration, continuous delivery and deployment.

# Criticism and Concerns:
> •	The microservices approach is subject to criticism for a number of issues:

> •	Services form information barriers.

> •	Inter-service calls over a network have a higher cost in terms of network latency and message processing time than in-process calls within a monolithic service process. 

> •	Testing and deployment are more complicated.

> •	Moving responsibilities between services is more difficult. It may involve communication between different teams, rewriting the functionality in another language or fitting it into a different infrastructure.However, Microservices can be deployed independently from the rest of the application while teams working on monoliths need to synchronize to deploy together.

> •	Viewing the size of services as the primary structuring mechanism can lead to too many services when the alternative of internal modularization may lead to a simpler design.This requires the use of applications helping understanding the overall architecture of the applications and interdependencies between components.

> •	Two-phased commits are regarded as an anti-pattern in microservices-based architectures as this results in a tighter coupling of all the participants within the transaction. However, lack of this technology causes awkward dances which have to be implemented by all the transaction participants in order to maintain data consistency.

> •	Development and support of many services is more challenging if they are built with different tools and technologies - this is especially a problem if engineers move between projects frequently.

> •	The protocol typically used with microservices (HTTP) was designed for public-facing services, and as such is unsuitable for working internal microservices that often must be impeccably reliable.

> •	While not specific to microservices, the decomposition methodology often uses functional decomposition, which does not handle changes in the requirements while still adds the complexity of services.

> •	The very concept of microservice is misleading, since there are only services. There is no sound definition of when a service starts or stops being a microservice.

# What does a Microservices Architecture Require?

> •	Loosely-coupled components

> •	API-accessible

> •	inter-component software access via a chosen protocol, HTTP being the most common 

The burgeoning "software-defined" world is all based around software speaking to software, abstracting the underlying infrastructure. Micro-services allows the isolation of roles and applications within that software environment to make them thinner, more agile, and also less dependent on each other at the code layer.

# Containers Does Not Mean Microservices:

Another challenge is that many folks have the idea that by using containers to build and deploy your applications that you have a microservices architecture. Nope.
Although containers are a great infrastructure platform to enable microservices, it does not always mean that. It is entirely possible to build a monolithic application inside containers. This is often compared to the idea that just because you drive an SUV, it doesn't mean that you are using it for sport utility. Sometimes it is just for comfort or style.

# Beyond Microservices:
	
Building a microservice-based application is more than just the technical aspects of it, we also have to consider the human side of deploying and delivering this type of application.
Having said that Microservice is a set of independently delivered and deployed services, each services has its own team. Typically, a team consists of 8 to 12 members, and can deliver and deploy their own service without contacting the other teams. This allows the team to be autonomous, as listed in one of its benefits.
A team is proportional to its service. Once the service becomes larger, the team building it becomes bigger. To conform to the standards of Microservice,the team has to be broken down into smaller groups and split the associated service or services.
When implementing a microservice-based application, we have to practice continuous delivery (such as Agile development) and deployment (such as Scrum deployment practices).

