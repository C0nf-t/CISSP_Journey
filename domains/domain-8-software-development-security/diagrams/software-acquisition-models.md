## Software Acquisition Models

Organizations generally have four primary ways to obtain software. Each approach offers different trade-offs in cost, control, security visibility, and development speed.

```mermaid
flowchart TD

A[Organization Needs Software]

A --> B[COTS<br>Commercial Off-The-Shelf]
A --> C[FOSS<br>Open Source Software]
A --> D[In-House Development]
A --> E[Outsourced Development]

B --> B1[Fast deployment]
B --> B2[Vendor support]
B --> B3[Limited code visibility]

C --> C1[Source code available]
C --> C2[Community collaboration]
C --> C3[Requires internal expertise]

D --> D1[Full control of features]
D --> D2[Custom security design]
D --> D3[Higher cost and development time]

E --> E1[External vendor builds software]
E --> E2[Scalable development resources]
E --> E3[Supply chain and security risks]

---

# How It Will Look Conceptually
            Organization Needs Software
                      |
 -------------------------------------------------
 |                |               |               |
 COTS FOSS In-House Outsourced
(Buy) (Open) (Build) (Contract)

---

# Why This Diagram Helps for CISSP

This visual helps remember the **decision trade-offs** tested in Domain 8:

| Model | Key Idea |
|-----|-----|
| **COTS** | Fast but limited control |
| **FOSS** | Transparent but requires expertise |
| **In-House** | Maximum control but expensive |
| **Outsourced** | Scalable but introduces supply chain risk |

---

# Senior Engineer Tip (Good for Your Notes)

You could add this small callout below the diagram:

```markdown
💡 **Senior Engineer Insight**

Most modern organizations actually use a **hybrid approach**.

For example:
- Core business logic may be **developed in-house**
- Infrastructure tools may be **open source**
- Business applications may be **COTS**
- Specialized components may be **outsourced**

The key is managing the **security risks and dependencies across all of them**.