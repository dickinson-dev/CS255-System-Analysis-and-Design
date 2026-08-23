# CS 255 System Analysis and Design | DriverPass

This repository presents my work from CS 255: System Analysis and Design at Southern New Hampshire University. The DriverPass case study required me to translate a client interview into documented business requirements, system workflows, UML models, and a technical design that could guide software development.

## Portfolio Artifacts

| Artifact | Focus |
| --- | --- |
| [Project One: Business Requirements Document](Project-One/Matthew-Dickinson-DriverPass-Business-Requirements-Document.pdf) | Business goals, functional and nonfunctional requirements, system limitations, user-interface needs, and project planning |
| [Project Two: System Design Document](Project-Two/Matthew-Dickinson-DriverPass-System-Design-Document.pdf) | Use case, activity, sequence, and class diagrams supported by hardware, software, development-tool, and infrastructure requirements |

## Project Reflection

### The Client and Requested System

DriverPass is a driver-training company that wanted a web-based system for both its customers and employees. Customers needed a way to purchase training packages, access learning materials, complete practice tests, schedule driving lessons, and review their progress. Employees needed tools for managing appointments, customer records, training content, reports, permissions, vehicles, and instructor assignments.

The proposed system combines these responsibilities into a single cloud-hosted application. It also supports outside payment and email services while keeping DriverPass responsible for reviewing DMV changes and publishing updated training content.

### What I Did Well

I did particularly well maintaining consistent operational rules as the project moved from written requirements into system models. For example, the lesson-reservation process checks the customer’s remaining package hours and verifies the availability of the customer, instructor, and vehicle before creating a reservation. Those same rules appear in the business requirements, activity diagram, sequence diagram, and class relationships.

I also made the requirements measurable where possible. The design identifies expected response times, availability goals, supported browsers, security controls, and the limits of the first release. This gives the development team clearer conditions for building and testing against.

### What I Would Revise

I would revise the use case diagram to make it easier to scan. The diagram captures a wide range of customer, employee, administrative, and outside-service interactions, but the number of connections makes portions of the model visually dense.

I would improve it by separating the customer-facing and administrative functions into supporting views, while retaining a single consolidated diagram for the complete system scope. This would make the responsibilities of each user group easier to understand without removing necessary relationships.

### Interpreting User Needs

I interpreted the client’s needs by turning statements from the interview into system behaviors, business rules, records, and constraints. The request for two-hour lessons became a fixed scheduling rule. Concerns about scheduling conflicts became availability checks for customers, instructors, and vehicles. Package limits were required to verify remaining lesson hours before accepting a reservation. The need for current training material became a controlled review and publishing process because the system does not receive automatic DMV updates.

Considering user needs is important because a system can function technically yet still fail to support the people who use it. Connecting each design decision to a real customer or employee task helps prevent missing workflows, unclear permissions, inconsistent records, and unnecessary features.

### My Approach to Software Design

I prefer to begin with the complete business process to understand the order of activities, decisions, exceptions, and handoffs. After the workflow is clear, I identify the objects and records needed to support it, including customers, packages, enrollments, reservations, vehicles, instructors, payments, test attempts, training content, and audit records. I then use behavioral models to check how those parts communicate during important tasks.

In future projects, I would continue using scenario walkthroughs, iterative diagram reviews, and comparisons between written requirements and system models. I would also use a formal requirements traceability matrix to confirm that every approved requirement appears in the design and can be connected to a future test.

## Skills Demonstrated

- Requirements gathering and stakeholder analysis
- Functional and nonfunctional requirement development
- Process and object modeling
- UML use case, activity, sequence, and class diagrams
- Scheduling and resource-conflict analysis
- Role-based access and security planning
- Cloud infrastructure and system-availability planning
- Communication of system designs to technical and nontechnical audiences

## Tools and Methods

- Lucidchart for UML diagrams and project scheduling
- Microsoft Word for requirements and design documentation
- GitHub for portfolio organization and version control
- Systems Development Life Cycle principles
- Process modeling and object-oriented analysis
