# CS 255: Systems Analysis and Design

This repository contains the foundational documents for the **DriverPass** system project, developed as part of my coursework for CS 255. The documents outline both the business requirements and the technical system design for a comprehensive driver training platform.

## Included Files
- `CS255_Business_Requirements.pages`: Outlines the project purpose, objectives, nonfunctional/functional requirements, and project timeline.
- `CS_255_System_Design_Document.pdf`: Details the technical architecture, database schemas, UI wireframes, and integration plans for the system.

---

## Project Reflection

**Briefly summarize the DriverPass project. Who was the client? What type of system did they want you to design?**
The DriverPass project involved designing a comprehensive cloud-based system to address gaps in current driver training and help students pass their DMV driving tests. The clients were Liam (the startup owner) and Ian (the IT officer). They wanted a web-based platform capable of handling tiered training packages, online courses and practice tests, and on-the-road driving reservations, complete with robust role-based access controls for admins, secretaries, drivers, and customers.

**What did you do particularly well?**
I was particularly successful at extracting clear, actionable requirements from the client interview and organizing them into distinct system components. I successfully bridged the gap between the business goals (like reducing DMV failure rates) and technical designs (like developing clear user roles and a structured database schema) to create a cohesive System Design Document.

**If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?**
If I could revise one part of my work, I would expand on the Nonfunctional Requirements section. While I covered the basics of security and platform constraints, I would improve it by defining more strict, measurable metrics for performance and scalability—such as specifying maximum acceptable page load times or the exact number of concurrent users the cloud infrastructure needs to support during peak registration hours.

**How did you interpret the user's needs and implement them into your system design? Why is it so important to consider the user's needs when designing?**
I interpreted the user's needs by carefully analyzing the specific pain points mentioned by Liam and Ian, such as the need for seamless scheduling and flexible learning packages. I implemented these into the design by focusing on an intuitive user interface, a centralized database for tracking reservations, and automated updates from the DMV. It is critical to consider the user's needs because software ultimately exists to solve human problems; if the design doesn't prioritize the end user's experience and workflow, the system will face poor adoption and fail to meet its business objectives.

**How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?**
My approach starts with a deep dive into requirements gathering and stakeholder analysis, followed by creating visual blueprints (like UML diagrams and wireframes) before any development begins. In the future, I plan to incorporate more iterative Agile techniques, such as scheduling regular feedback loops with stakeholders to review intermediate design mockups, ensuring that the architecture remains aligned with evolving business needs throughout the project lifecycle.
