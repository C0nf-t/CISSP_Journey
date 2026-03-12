# Domain 8 – Software Development Security
## Software Development Lifecycle (SDLC)

---

## What the SDLC Really Is

The **Software Development Lifecycle (SDLC)** is the structured process organizations follow to design, build, test, and deploy software.

Think of it as the **roadmap for turning an idea into a working application**.

Every organization implements SDLC slightly differently, but the core goal is the same:

> Build software in a structured, predictable way so it works reliably and securely.

Without a defined lifecycle, development becomes chaotic — which leads to bugs, outages, and security vulnerabilities.

From a **security perspective**, SDLC matters because modern organizations rely heavily on software, and insecure software quickly becomes an attack surface.

---

## The Major Phases of SDLC

Most SDLC models follow five major phases:

1. Requirements
2. Design
3. Development
4. Testing
5. Deployment

Each phase builds on the previous one.

---

# 1. Requirements Phase

This phase defines **what the application is supposed to do**.

The team gathers information from stakeholders, customers, and business leaders to understand the problem the software should solve.

### Key Questions

- What features must the application provide?
- Who will use it?
- What data will it handle?
- What regulations or security requirements apply?

### Example

Imagine a company building an **e-commerce application**.

Functional requirements might include:

- Users can create accounts
- Users can search for products
- Users can purchase items
- Admins can manage inventory

Security requirements should also be defined here:

- Password complexity
- Multi-factor authentication
- Encryption for payment data
- Logging and monitoring

A senior engineer will always emphasize:

> If security requirements are not defined early, they usually get ignored later.

---

# 2. Design Phase

Once requirements are understood, the team creates the **system architecture**.

This phase defines **how the system will work**.

Think of it like the **architectural blueprint of a building**.

### Design Considerations

- Application architecture
- Database structure
- Authentication mechanisms
- Network communication
- Infrastructure requirements

### Example Architecture

For an e-commerce platform:

- Frontend web application
- Backend API services
- Database for product and user data
- Payment processing service
- Authentication system

### Security Activities in Design

Security should be built in during this stage through:

- **Threat modeling**
- **Security architecture design**
- **Trust boundary analysis**
- **Security training for developers**

Example senior engineer question:

> “If this API is exposed to the internet, what prevents abuse or unauthorized access?”

Decisions made during design often determine the **long-term security posture of the application**.

---

# 3. Development Phase

This is where developers begin **writing the actual code**.

Tasks are typically broken into modules and distributed across development teams.

Developers follow coding standards and use tools such as:

- Compilers
- Debuggers
- Integrated Development Environments (IDEs)

This is usually **the longest phase of the SDLC**.

### Example: Login Feature

A poorly written login query might look like:


SELECT * FROM users WHERE username='input' AND password='input'



This introduces **SQL injection vulnerabilities**.

Secure coding practices would instead include:

- Parameterized queries
- Input validation
- Authentication frameworks
- Secure password hashing

### Security Practices During Development

Security teams typically introduce tools such as:

- **Static Application Security Testing (SAST)**
- Dependency vulnerability scanning
- Secure coding guidelines
- Code reviews

A common lesson senior engineers share:

> If insecure code is written, no firewall will save the application.

---

# 4. Testing Phase

Once the software is built, it enters **testing**.

The goal is to ensure the system works properly and meets the original requirements.

Testing teams validate:

- Functional behavior
- System performance
- Error handling
- Integration with other systems

If defects are discovered, they are reported to developers for fixes.

This process continues until the software is stable.

### Security Testing

Security validation during testing may include:

- Penetration testing
- Dynamic Application Security Testing (DAST)
- Vulnerability scanning

### Example

A penetration tester might discover:

- Unauthenticated API endpoints
- Sensitive information leakage
- Weak session tokens
- Improper input validation

Finding these issues before production significantly reduces risk.

---

# 5. Deployment Phase

Once testing is complete, the application is released into the **production environment**.

At this stage, the application becomes available to real users.

Deployment typically includes:

- Installing the application on production servers
- Configuring infrastructure
- Integrating external services
- Enabling monitoring

### Security Responsibilities During Deployment

Security teams ensure:

- Secure server configuration
- System hardening
- Vulnerability scanning
- Logging and monitoring

Example deployment checks:

- TLS encryption enabled
- Default credentials removed
- Firewall rules configured
- Security monitoring enabled

Deployment is not just about launching software — it’s about launching it **securely**.

---

# Secure Software Development Lifecycle (SSDLC)

The **Secure Software Development Lifecycle (SSDLC)** integrates security into every phase of development.

Security is not treated as an afterthought but as a core component of the system.

| SDLC Phase | Security Activity |
|-------------|------------------|
| Requirements | Define security requirements and perform risk assessments |
| Design | Conduct threat modeling and design secure architecture |
| Development | Apply secure coding practices and run static code analysis |
| Testing | Perform penetration testing and dynamic security testing |
| Deployment | Harden systems and perform vulnerability scanning |

SSDLC requires collaboration between:

- Developers
- Security engineers
- System administrators
- Operations teams

---

# Why Secure SDLC Matters

Integrating security throughout development provides several benefits:

- Improves overall software security
- Detects vulnerabilities earlier
- Reduces remediation costs
- Speeds up deployment timelines
- Reduces organizational risk

A common rule in security engineering:

> The earlier a vulnerability is discovered, the cheaper it is to fix.

A vulnerability discovered during design may take minutes to resolve.

The same vulnerability discovered in production could require weeks of remediation.

---

# Real-World Analogy

Think of building a house.

| SDLC Phase | House Equivalent |
|-------------|-----------------|
| Requirements | Deciding what kind of house to build |
| Design | Creating architectural blueprints |
| Development | Construction |
| Testing | Home inspections |
| Deployment | People move in |

Secure SDLC is like ensuring:

- Doors have locks
- Electrical systems are safe
- Windows are reinforced
- Alarm systems are installed

Security should be **designed into the structure**, not added afterward.

---

# Key Takeaway

Secure software is not created by security teams alone.

It requires collaboration between:

- Developers
- Architects
- Operations teams
- Security engineers

When security is integrated throughout the lifecycle, organizations can build software that is **both functional and resilient against attacks**.
