# NHS Waiting Time Database System

This project presents the design of a relational database system aimed at improving
the monitoring and management of NHS hospital waiting times across the UK.

The system was designed as part of a university coursework project and focuses on
accurate data modelling, normalization, and realistic healthcare use cases.

📄 **Full technical report:**  
See `CW2-NHS-WAITING-TIME-PROJ.pdf` for the complete requirement analysis, ER diagrams,
logical model, and normalization discussion.

The UK Government identified significant issues within existing NHS data systems,
including lost or inconsistent patient records and delays caused by poor data sharing
between hospitals, GPs, and consultants.

This project addresses those issues by designing a robust relational database capable
of:
- Accurately tracking patients, hospitals, and waiting lists
- Supporting regional analysis across countries, counties, and districts
- Enabling realistic analytical queries to identify healthcare demand
- Maintaining data consistency, integrity, and confidentiality

- Design a normalized relational database reflecting real NHS structures
- Model the UK's regional healthcare hierarchy (Country → County → District)
- Track patients, hospitals, admissions, appointments, and waiting lists
- Support analytical queries such as:
  - Identifying regions with high healthcare demand
  - Monitoring waiting list sizes per county
- Ensure the design is scalable and adaptable for future NHS requirements

The database design follows a structured methodology:
1. Requirement analysis based on NHS operational needs
2. Conceptual modelling using an Entity-Relationship (ER) diagram
3. Conversion to a logical relational model
4. Normalization to Third Normal Form (3NF) to eliminate redundancy

- Country, County, District
- Hospital
- Patient, PatientAddress
- Admission
- Appointment
- Procedure
- WaitingList
- FirstMinister
- MinisterStatement

The database was normalized to Third Normal Form (3NF):
- 1NF: All attributes are atomic and uniquely identifiable
- 2NF: All non-key attributes fully depend on the primary key
- 3NF: No transitive dependencies remain

This ensures:
- Reduced data redundancy
- Improved data integrity
- Easier long-term maintenance and scalability

The database supports realistic NHS-style queries, including:
- Identifying districts or counties with high patient demand
- Monitoring waiting lists by region or hospital
- Analysing admissions and appointment volumes
- Supporting government-level resource allocation decisions

- SQL
- Relational Database Design
- Entity-Relationship Modelling
- Normalization (1NF, 2NF, 3NF)
- Data Integrity & Consistency

Salman Hussain  
BSc Computer Science – Queen Mary University of London

This repository focuses on database design rather than application-level implementation.
The accompanying PDF contains the full academic justification, diagrams, and design
decisions behind the system.
