# Software Security Testing

## Why Security Testing Matters

When developers build applications, bugs are inevitable. Some bugs are harmless, but others create **security vulnerabilities** that attackers can exploit.

If vulnerabilities make it into production, they can lead to:

- data breaches
- unauthorized access
- service outages
- compliance violations

Because of this, modern development teams integrate **security testing throughout the Software Development Lifecycle (SDLC)**.

Several testing methods help identify vulnerabilities at different stages of development, including:

- Static Application Security Testing (SAST)
- Dynamic Application Security Testing (DAST)
- Interactive Application Security Testing (IAST)
- Software Composition Analysis (SCA)

Each method identifies different types of security issues.

---

# Static Application Security Testing (SAST)

Static Application Security Testing is commonly referred to as **white-box testing**.

SAST analyzes the **source code of an application without running the program**. The testing tool scans the code for patterns that may indicate security vulnerabilities. :contentReference[oaicite:0]{index=0}

Because SAST reviews the code itself, it can identify vulnerabilities **early in the development lifecycle**, often during the coding phase.

Think of SAST like reviewing the **blueprints of a building before construction is finished**.

### What SAST Can Detect

SAST tools can detect issues such as:

- SQL injection vulnerabilities
- buffer overflows
- insecure input validation
- weak authentication logic
- insecure error handling

### Example

Imagine a developer writes a function that directly inserts user input into a database query.

A SAST tool scans the source code and flags a potential **SQL injection vulnerability** because the input is not sanitized.

Since this issue is caught early, the developer can fix it before the application is deployed.

---

# Dynamic Application Security Testing (DAST)

Dynamic Application Security Testing is known as **black-box testing**.

Instead of reviewing source code, DAST tools test the application **while it is running**.

These tools interact with the application the same way an attacker might, sending requests and analyzing responses to identify vulnerabilities. :contentReference[oaicite:1]{index=1}

Think of DAST like testing a car **after it has been built**, driving it on the road to see how it performs.

### What DAST Can Detect

DAST tools can find issues such as:

- authentication weaknesses
- misconfigured servers
- exposed APIs
- cross-site scripting (XSS)
- SQL injection attacks

Because DAST requires a running application, it usually occurs **later in the development lifecycle**, often during staging or pre-production testing.

### Example

A DAST tool might scan a running web application and discover that certain API endpoints can be accessed without authentication.

This issue may not have been visible directly in the source code but becomes clear during runtime testing.

---

# Interactive Application Security Testing (IAST)

Interactive Application Security Testing combines elements of both **SAST and DAST**.

IAST tools monitor an application **while it is running**, but they also analyze what is happening inside the application during execution.

This means IAST tools can observe how code behaves in real time and identify vulnerabilities more precisely.

### How IAST Works

IAST tools typically integrate into the application runtime environment or testing environment. As the application runs, the tool analyzes:

- data flow through the application
- executed code paths
- runtime vulnerabilities

Because it operates inside the application, IAST can often identify vulnerabilities more accurately than traditional black-box testing.

### Example

If a user input travels through several functions before reaching a database query, an IAST tool can track that entire path and identify whether the input is properly sanitized before being used.

---

# Software Composition Analysis (SCA)

Modern applications rarely rely entirely on custom code. Most software projects use **third-party libraries and open-source components**.

Software Composition Analysis focuses on identifying security risks in those external dependencies.

SCA tools analyze the software components used in an application and compare them against vulnerability databases.

### What SCA Detects

SCA tools help identify:

- vulnerable open-source libraries
- outdated dependencies
- licensing risks
- supply chain vulnerabilities

### Example

A developer includes an open-source encryption library in an application.

Later, a vulnerability is discovered in that library. An SCA tool detects that the project is using the vulnerable version and alerts the development team so they can upgrade to a patched version.

---

# Comparing Security Testing Methods

| Method | Description | When Used |
|------|-------------|-----------|
| SAST | Analyzes source code to find vulnerabilities | Early development |
| DAST | Tests running applications for vulnerabilities | Later stages or staging environments |
| IAST | Monitors application behavior during execution | Testing or runtime environments |
| SCA | Analyzes third-party dependencies and libraries | Throughout development |

Each method provides a different perspective on application security.

---

# Why Modern Teams Use Multiple Testing Methods

No single testing method can detect every vulnerability.

SAST may detect insecure code patterns, but it cannot detect runtime configuration problems.

DAST can identify runtime issues but cannot analyze internal code structure.

SCA focuses on vulnerabilities in external libraries.

IAST provides deeper insight into how applications behave during execution.

Because of this, mature development teams combine multiple security testing methods to gain **complete visibility into application security risks**.

---

# Real-World Example

Imagine a company developing an online banking platform.

During development:

- A **SAST tool** scans the code and finds input validation issues.

During testing:

- A **DAST tool** scans the running application and discovers exposed endpoints.

During runtime testing:

- An **IAST tool** monitors data flow and identifies unsafe database queries.

During dependency analysis:

- An **SCA tool** detects that an open-source library used in the application contains a known vulnerability.

Each tool finds different issues, helping the organization strengthen its overall security posture.

---

# Senior Engineer Takeaway

When mentoring junior engineers, I often explain security testing like this:

Different testing methods look at the application from different angles.

- SAST reviews the code.
- DAST tests the running system.
- IAST analyzes behavior during execution.
- SCA examines third-party components.

Using these methods together helps development teams catch vulnerabilities earlier and build **more secure and resilient applications**.