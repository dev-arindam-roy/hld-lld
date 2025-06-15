
In software development, the terms High-Level Design (HLD) and Low-Level Design (LLD) refer to two distinct stages in the design phase of the software development lifecycle. Each focuses on a different level of detail and abstraction.

# High-Level Design (HLD)
High-Level Design provides a system-wide view of the architecture and outlines how the system will be structured.

### Key Characteristics:
- Abstract / Architectural view
- Identifies modules, components, and interactions
- Defines technology stack and architecture patterns (e.g., MVC, microservices)
- Specifies data flow between modules
- Includes external integrations (e.g., databases, APIs, services)
- Addresses non-functional requirements (e.g., scalability, performance, security)

### Typical Artifacts:
- Architecture Diagrams
- Component Diagrams
- ER Diagrams (Entity-Relationship)
- System Flow Charts

### Example:
For a CRM system:

- Modules: User Management, Leads Management, Sales Dashboard
- Technologies: Laravel for backend, React for frontend, MySQL for database
- Architecture: RESTful API, Role-based Access Control

# Low-Level Design (LLD)
Low-Level Design dives into the detailed internal logic of the individual components specified in HLD.

### Key Characteristics:
- Detailed design for developers to start coding
- Describes class names, methods, parameters, and data types
- Includes database schema, pseudocode, algorithms
- Often language-specific
- Focuses on implementation logic and error handling

### Typical Artifacts:
- Class Diagrams
- Sequence Diagrams
- Detailed Flow Charts
- Function Specifications

### Example:
For the "**Leads Management**" module:

- Class: LeadController
- Methods: createLead(Request $req), assignToSalesperson()
- Database Tables: leads, lead_statuses
- Validation Rules: Required fields, unique email, date format check

# Summary Table:

| Feature        | High‑Level Design (HLD)                           | Low‑Level Design (LLD)                           |
|----------------|---------------------------------------------------|--------------------------------------------------|
| Focus          | System architecture & module breakdown            | Internal logic & detailed design                 |
| Audience       | Architects, Tech Leads, Stakeholders              | Developers                                       |
| Detail Level   | Abstract / Overview                               | Concrete / In‑depth                              |
| Output         | Component diagrams, tech stack, architecture docs | Class diagrams, pseudocode, DB schemas           |
| Example        | API Gateway routes to microservices               | Method to calculate discount for order item      |

**If you're building a software system, HLD comes before LLD. HLD sets the blueprint, while LLD provides the engineering plan to build each piece.**
