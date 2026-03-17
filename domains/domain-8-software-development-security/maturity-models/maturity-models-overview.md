# Maturity Models

When people first hear the term **maturity model**, it can sound overly academic. In reality, the idea is pretty simple.

A maturity model is a framework used to measure **how disciplined and structured an organization's development processes are**.

Think of it like evaluating the growth of an engineering team.

An immature development environment usually looks like this:

- Developers working in isolation
- Processes changing from project to project
- Security reviews happening only after something breaks
- Documentation that barely exists

A mature environment looks very different:

- Development processes are standardized
- Security practices are integrated early
- Testing and automation are consistent
- Decisions are guided by metrics and continuous improvement

The key idea behind maturity models is this:

> The quality of the software produced by an organization is directly related to the quality of the processes used to build it.

As processes mature, software becomes **more reliable, more secure, and more predictable.**

---

# Capability Maturity Model (CMM)

The **Capability Maturity Model (CMM)** was introduced by the **Software Engineering Institute in 1991** to help organizations improve their software development processes.

It provides a way to measure how mature an organization’s development process is and identify areas for improvement.

CMM defines **five levels of maturity**.

A simple acronym to remember them is:
IRDMO

Initial  
Repeatable  
Defined  
Managed  
Optimizing

You can think of these levels as a progression from **chaotic development → disciplined engineering processes**.

---

## Level 1 – Initial

At this stage, development processes are **unpredictable and poorly controlled**.

Work gets done mostly because of individual effort rather than structured processes.

Typical characteristics:

- No standard development process
- Minimal documentation
- Success depends on individual developers
- Problems are solved reactively

### Example

Imagine a startup where developers push code directly to production without testing.

Things might work for a while, but the environment is fragile. If one key developer leaves, the team may struggle to maintain the system.

---

## Level 2 – Repeatable

At the repeatable level, organizations begin introducing **basic project management and documentation practices**.

Processes are defined enough that successful work can be **repeated across projects**.

Improvements often include:

- Version control systems
- Change management procedures
- Basic documentation
- Defined development workflows

### Example

A company introduces pull requests and code reviews before changes are merged.

Now development becomes more consistent and easier to track.

---

## Level 3 – Defined

At this stage, development processes become **standardized across the organization**.

Instead of every team doing things differently, the organization follows a **common development framework**.

Typical characteristics:

- Documented development standards
- Organization-wide engineering practices
- Standardized project management

### Example

A company creates a formal **Software Development Lifecycle (SDLC)** policy that every project must follow.

This ensures development practices remain consistent across teams.

---

## Level 4 – Managed

At the managed level, organizations begin **measuring their development processes using data and metrics**.

Processes are now **quantitatively controlled and predictable**.

Metrics may include:

- defect rates
- vulnerability counts
- testing coverage
- time to resolve bugs

### Example

A security team tracks how long it takes to remediate vulnerabilities discovered during testing.

Leadership uses these metrics to improve development practices.

---

## Level 5 – Optimizing

This is the most mature stage.

Organizations at this level focus on **continuous improvement**.

Processes are regularly evaluated and improved using new tools, automation, and lessons learned.

### Example

A mature organization might have:

- automated CI/CD pipelines
- automated security scanning
- continuous testing
- DevSecOps practices

Security becomes a **built-in part of development**, not something added later.

---

# Capability Maturity Model Integration (CMMI)

**CMMI** is essentially the evolution of the original CMM model.

It integrates multiple improvement models into a single framework designed to help organizations improve:

- product development
- service delivery
- project management
- engineering practices

If CMM introduced the concept of process maturity, **CMMI expanded it into a broader organizational improvement framework**.

CMMI uses the same **five maturity levels**:

| Level | Description |
|------|-------------|
| 1 | Initial – Processes are unpredictable |
| 2 | Managed – Basic project management practices exist |
| 3 | Defined – Processes are standardized across the organization |
| 4 | Quantitatively Managed – Processes are measured and controlled |
| 5 | Optimizing – Continuous improvement is emphasized |

### Real-world perspective

Two companies may produce similar software.

A **low maturity organization** might constantly struggle with delays, bugs, and inconsistent development practices.

A **high maturity organization** will have predictable development cycles, strong testing practices, and clear process improvements over time.

The difference is **process discipline.**

---

# OpenSAMM (Software Assurance Maturity Model)

**OpenSAMM**, often simply called **SAMM**, is a maturity model specifically designed for **software security**.

It was developed by **OWASP** to help organizations evaluate and improve their application security practices.

Unlike CMM or CMMI, which focus on development process maturity, OpenSAMM focuses on **how well security is integrated into the development lifecycle.**

It works with any development model, including:

- Waterfall
- Agile
- DevOps

This flexibility makes it especially useful in modern development environments.

---

## OpenSAMM Maturity Levels

OpenSAMM uses **four maturity levels**.

| Level | Meaning |
|------|---------|
| 0 | No formal security practices |
| 1 | Initial security practices introduced |
| 2 | Security practices are defined and consistently applied |
| 3 | Security practices are optimized and continuously improved |

Each level represents how deeply security is embedded into development practices.

---

## OpenSAMM Core Business Functions

OpenSAMM organizes software security activities into five major functions.

---

### Governance

Governance focuses on **how an organization manages software security at a strategic level**.

Examples include:

- security policies
- security metrics
- compliance programs
- developer security training

---

### Design

Design focuses on building **secure system architecture from the beginning**.

Activities include:

- threat modeling
- defining security requirements
- designing secure architectures

---

### Implementation

Implementation focuses on how software is actually built.

Key activities include:

- secure coding practices
- secure build pipelines
- defect management

This area directly impacts developers' day-to-day work.

---

### Verification

Verification ensures security controls actually work.

Activities include:

- security testing
- architecture reviews
- requirements-based testing

This stage helps detect vulnerabilities before deployment.

---

### Operations

Operations focuses on maintaining security **after software is deployed**.

This includes:

- incident response
- monitoring
- environment management

Security must continue throughout the application's lifecycle.

---

# Quick Comparison of Maturity Models

| Model | Focus |
|------|------|
| CMM | Improving software development processes |
| CMMI | Expanded framework for organizational process improvement |
| OpenSAMM | Improving software security maturity |

A simple way to remember this for CISSP:

- **CMM / CMMI → development process maturity**
- **SAMM → security maturity**

---

# Senior Engineer Takeaway

When mentoring junior engineers, I often explain maturity models like this:

Early-stage organizations rely heavily on **talented individuals solving problems as they appear**.

Mature organizations rely on **well-designed processes that prevent problems from happening in the first place**.

As an organization's maturity increases:

- development becomes more predictable
- security becomes integrated earlier
- defects decrease
- risk decreases

In short, maturity models help organizations move from **reactive firefighting to disciplined engineering practices.**