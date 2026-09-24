CyberHelp Plan Prompt

We will now complete the docs/design/plan.md file for the CyberHelp application.

Use these files as the source of truth:

docs/design/specification.md
docs/design/plan.md
docs/design/reference/plan-guide.md

The specification has already been completed and contains requirements R1 through R10. The plan must explain how the CyberHelp application will be built without changing the requirements or inventing new features.

CyberHelp is a simple web application that helps people find understandable information about common cybersecurity and technical problems.

The main user flow is:

Home → Category → Topic → Problem Information → Recommended Steps

Important requirements

Every major decision, component, and plan item must trace back to one or more requirement IDs from the specification.

Use the existing requirement IDs:

R1: When a user opens CyberHelp, the system shall show the available categories.
R2: When a user selects a category, the system shall show the topics in that category.
R3: When a user selects a topic, the system shall show information about the problem.
R4: When a topic is shown, the system shall show a description of the problem.
R5: When available, the system shall show common warning signs.
R6: When available, the system shall show recommended steps.
R7: The system shall provide a way for the user to return to the previous page.
R8: If a category has no topics, the system shall show a message explaining that information is not available.
R9: The system shall use simple labels and navigation.
R10: The system shall not ask users for passwords or other sensitive information.
Approach

CyberHelp should be developed as a simple front-end web application using standard HTML, CSS, and JavaScript.

The first version should focus on the front-end prototype rather than accounts, databases, live cybersecurity monitoring, automatic malware detection, payments, or other features that are outside the specification.

The application should use categories and topics to organize the information. Users should be able to select a category, select a topic, read information about the problem, view warning signs when available, view recommended steps when available, and navigate back.

Tech Stack

Use:

Frontend: HTML, CSS, JavaScript
Data: Static JavaScript data/objects for the prototype
Hosting: GitHub Pages
Backend/DB: None for the first version
Other services/APIs: None required for the first version
Plan requirements

Complete docs/design/plan.md using the existing template and the plan guide.

Do not change the structure of the template unnecessarily.

Complete these sections:

Approach Summary
Tech Stack
Key Decisions (ADRs)
Components / Building Blocks
Dependencies & Assumptions
Risks
Sequencing
Review & Approval

For the ADR section, document meaningful technical choices and include at least one real alternative that was considered for each decision.

For Components, identify the major pieces of CyberHelp, such as:

Home/category view
Category/topic view
Problem information view
Recommended steps section
Navigation/back controls
CyberHelp content data

For risks, consider issues such as unclear category names, users having difficulty finding recommended steps, navigation confusion, incomplete cybersecurity information, and the possibility of the project becoming too large.

For sequencing, prioritize building the basic navigation and content flow first, then improving the presentation and testing the application.

Do not add user accounts, databases, live support, malware scanning, payments, or automatic cybersecurity tools because those are outside the current specification.

Do not change specification.md.

Before finishing, check the completed plan against docs/design/reference/plan-guide.md.

Make sure:

Every ADR has a requirement ID.
Every component has a requirement ID.
Every risk has a mitigation.
Sequencing explains what is built first and why.
Review and approval are not falsely marked as approved.
The plan remains simple enough for a college web programming project.

Write the completed content directly into docs/design/plan.md.