## Hibernate Many to Many
> **A many-to-many relationship occurs when multiple records in a table are associated with multiple records in another table. For example, a many-to-many relationship exists between employees and projects.**

![many-to-many relationship](https://www.baeldung.com/wp-content/uploads/2017/09/New.png)

- In this, any given employee can be assigned to multiple projects and a project may have multiple employees working for it, leading to a `many-to-many` association between the two.

- You also need to create the employee and project tables along with the employee_project join table with employee_id and project_id as foreign keys. That's mean, you need to create a new two classes for the employee and for the project.

### Threats and solutions

> **What is Threat Modeling?**
> *Threat modeling is a proactive strategy for evaluating risks. It involves identifying potential threats, and developing tests or procedures to detect and respond to those threats. This involves understanding how threats may impact systems, classifying threats and applying the appropriate countermeasures*.

- **Threat models can be like:**
1. Organized criminals breaking into your email account and sending spam using your identity. So, Strong passwords + common, sense (don’t click on unsolicited herbal Viagra ads that result in keyloggers and sorrow)

2. The Mossad can do Mossad things with your email account.

### Resources
- https://www.baeldung.com/hibernate-many-to-many
- http://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf
- https://www.exabeam.com/information-security/threat-modeling/