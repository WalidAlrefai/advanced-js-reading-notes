# Class 11

# Event Driven Applications

## What's an event?
An event is any significant occurrence or change in state for system hardware or software. An event is not the same as an event notification, which is a message or notification sent by the system to notify another part of the system that an event has taken place.

The source of an event can be from internal or external inputs. Events can generate from a user, like a mouse click or keystroke, an external source, such as a sensor output, or come from the system, like loading a program.

## How does event-driven architecture work?
Event-driven architecture is made up of event producers and event consumers. An event producer detects or senses an event and represents the event as a message. It does not know the consumer of the event, or the outcome of an event. 

After an event has been detected, it is transmitted from the event producer to the event consumers through event channels, where an event processing platform processes the event asynchronously. Event consumers need to be informed when an event has occurred. They might process the event or may only be impacted by it. 

The event processing platform will execute the correct response to an event and send the activity downstream to the right consumers. This downstream activity is where the outcome of an event is seen. 

Apache Kafka is a distributed data streaming platform that is a popular event processing choice. It can handle publishing, subscribing to, storing, and processing event streams in real time. Apache Kafka supports a range of use cases where high throughput and scalability are vital, and by minimizing the need for point-to-point integrations for data sharing in certain applications, it can reduce latency to milliseconds. 

There are other middleware event managers available that can serve as an event processing platform.

## Event-driven architecture models
An event driven architecture may be based on either a pub/sub model or an event stream model.

### Pub/sub model
This is a messaging infrastructure based on subscriptions to an event stream. With this model, after an event occurs, or is published, it is sent to subscribers that need to be informed.

### Event streaming model
With an event streaming model, events are written to a log. Event consumers don’t subscribe to an event stream. Instead, they can read from any part of the stream and can join the stream at any time. 

There are a few different types of event streaming:

  - Event stream processing uses a data streaming platform, like Apache Kafka, to ingest events and process or transform the event stream. Event stream processing can be used to detect meaningful patterns in event streams.
  - Simple event processing is when an event immediately triggers an action in the event consumer.
  - Complex event processing requires an event consumer to process a series of events in order to detect patterns.
## Benefits of event-driven architecture
An event-driven architecture can help organizations achieve a flexible system that can adapt to changes and make decisions in real time. Real-time situational awareness means that business decisions, whether manual or automated, can be made using all of the available data that reflects the current state of your systems. 

Events are captured as they occur from event sources such as Internet of Things (IoT) devices, applications, and networks, allowing event producers and event consumers to share status and response information in real time. 

Organizations can add event-driven architecture to their systems and applications to improve the scalability and responsiveness of applications and access to the data and context needed for better business decisions.

## The question

1- **Why is access control important ?**

Access control is important because it is a valuable security technique that can be used to regulate who or what can view or use any given resource. In an I.T security setting this could translate to who can access and edit a particular file, what kinds of equipment can be used or who can access certain devices.

2- **Describe an application that would need access control?**

roles are required for an extreme programming project to work and the persons who take these roles take the corresponding responsibilities and are accountable for their contribution to these roles. It is advised to allocate the right people for the roles rather than trying to change the people to fit into those roles.

3- **What is a role used for?**

Role-based access control (RBAC), also known as role-based security, is an access control method that assigns permissions to end-users based on their role within your organization. RBAC provides fine-grained control, offering a simple, manageable approach to access management that is less error-prone than individually assigning permissions.

4- **Why is role based access control more scalable than discretionary or mandatory access control?**

1. DAC is the way to go to let people manage the content they own. It might sound obvious, but for instance DAC is very good to let users an online social network choose who accesses their data. It allows people to revoke or forward privileges easily and immediately. Reactive access control, Seeing further and Laissez-faire file sharing provide nice examples of research on DAC with users.

2. RBAC is a form of access control which as you said is suitable to separate responsibilities in a system where multiple roles are fulfilled. This is obviously true in corporations (often along with compartmentalization e.g. Brewer and Nash or MCS) but can also be used on a single user operating system to implement the principle of least privilege. RBAC is designed for separation of duties by letting users select the roles they need for a specific task. The key question is whether you use roles to represent tasks performed on your system and assign roles in a central authority (in which case RBAC is a form of MAC); or if you use roles to let users control permissions on their own objects (leading to multiple roles per object and absolutely no semantics in roles, even though it's theoretically possible).

3. MAC in itself is vague, there are many many ways to implement it for many systems. In practice, you'll often use a combination of different paradigms. For instance, a UNIX system mostly uses DAC but the root account bypasses DAC privileges. In a corporation, beyond separating your different departments and teams with MAC/RBAC you may allow some DAC for coworkers to share information on your corporate file system.

## Terms:
### Authorization
Authorization is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular.

### Role Based Access Control
is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control (MAC) or discretionary access control (DAC).

### Capabilities
A capability is a communicable, unforgettable token of authority. It refers to a value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object.