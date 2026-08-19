The Final Causal Model (Joint Statement)Business Decision: In 1999, the UK Post Office and the government decided to roll out the Horizon system across thousands of branches despite knowing the system was unstable, driven by political pressure.
Process Failure: Post Office management and Fujitsu aggressively suppressed system defects, lacked independent technical auditing, and maintained a toxic culture that trusted the computer while distrusting human operators.
Engineering Defect: The system contained severe software bugs (like the "Callendar Square" and "Dalmellington" bugs), race conditions, synchronization errors, and an architecture that allowed Fujitsu remote access to alter branch accounts silently.
Loss: Over 900 innocent sub-postmasters were wrongfully convicted, leading to over £1 billion in financial losses, bankruptcies, wrongful imprisonment, and at least four suicides.
Technical Root Causes 
C1: Requirements Failure: Missing requirements for a transparent audit trail and incomplete handling of interrupted network states.
C2: Assumption Failure: The incorrect assumption that the central database was inherently infallible and discrepancies were exclusively user error.
C3: Design / Architecture Failure: Allowed remote access to local branch data without operator knowledge or digital signatures.
C4: Implementation Failure: Severe programming defects, including duplicate database entries and unhandled race conditions.
C5: The software suffered from incredibly poor integration and regression testing. Fixes deployed for one bug frequently introduced new errors into the system.
C6: Configuration / Change-Management Failure: Uncontrolled, undocumented manual changes to live databases to "fix" discrepancies.
C7: Deployment / Operational Failure: Deployed across 18,000 branches despite known bugs, with inadequate operational monitoring.
Organizational / Process Causes
C8: The system created massive automation bias, where Post Office investigators and UK courts implicitly trusted the computer's output over human testimony. Additionally, the software featured misleading interfaces that literally forced sub-postmasters to digitally "accept" false financial shortfalls just so they could open their branches for business the next morning.
C9: Management exhibited insufficient technical oversight, weak defect management, poor escalation of technical problems, poor handling of user complaints, and an excessive reliance on Horizon's figures.
C10: Both Fujitsu and Post Office management engaged in a massive concealment of system limitations. Fujitsu engineers acting as expert witnesses in court failed to communicate the known risks and bugs to the judges. This was a direct failure to escalate concerns and a catastrophic breach of the professional duty to protect the public from an unsafe system.
