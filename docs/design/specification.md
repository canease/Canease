# CyberHelp — Specification

## 0. Constitution

- CyberHelp must be simple and easy for beginners to use.
- Information must be organized into clear categories.
- Instructions must use plain language and provide practical next steps.
- CyberHelp must not ask users to enter passwords or other sensitive information.
- Cybersecurity information should use reliable sources, such as government cybersecurity resources.

## 1. Problem & Intent

### Who is this for?

CyberHelp is for people who need help understanding common cybersecurity and technical problems, especially people who may not have much technical experience.

### What problem does it solve?

People often struggle to find simple and reliable information about cybersecurity problems because they have to search through multiple websites. Some websites use technical language or provide conflicting advice, making it difficult to know what to do.

CyberHelp will organize common problems into categories and provide descriptions, warning signs, and recommended steps in one place.

### What does success look like?

The project will be considered successful when:

- Users can identify a category that matches their problem.
- Users can find information about a topic without searching multiple websites.
- Users can find the recommended steps within two minutes during a basic usability test.
- Users can move between the homepage, categories, and topics without getting lost.
- Users can understand the instructions without needing advanced technical knowledge.

## 2. Scope

### In Scope

- A homepage displaying cybersecurity and technical support categories.
- Categories with clearly labeled topics.
- Basic descriptions of common problems.
- Common warning signs.
- Clearly labeled recommended steps.
- Back buttons that allow users to return to the previous screen or homepage.
- Helpful messages when information is unavailable.
- Simple navigation and readable text.
- Information based on reliable sources, including the FTC and CISA.

### Out of Scope

- Live technical support.
- Automatically fixing computer or cybersecurity problems.
- Performing malware removal.
- Live cybersecurity monitoring.
- User accounts and login systems.
- Payments or subscriptions.
- Collecting passwords or other sensitive personal information.
- Advanced diagnostic tools.

## 3. User Scenarios

### Scenario 1: Find a Help Topic

**Actor:** User

**Trigger:** The user has a cybersecurity or technical problem.

**Steps:**
1. Open CyberHelp.
2. Review the available categories.
3. Select a category that matches the problem.
4. Select a topic within that category.

**Success Outcome:** The user finds information relevant to the problem.

**Failure Outcome:** The user cannot find a matching category or topic and needs a clear message explaining that the information is unavailable.

### Scenario 2: Understand a Problem

**Actor:** User

**Trigger:** The user selects a help topic.

**Steps:**
1. Read the problem description.
2. Review the common warning signs.
3. Decide whether the information may apply to the situation.

**Success Outcome:** The user understands the general problem and its warning signs.

**Failure Outcome:** The information is confusing, incomplete, or does not help the user understand the problem.

### Scenario 3: Find Recommended Steps

**Actor:** User

**Trigger:** The user wants to know what to do about a problem.

**Steps:**
1. Open the relevant help topic.
2. Find the Recommended Steps section.
3. Read the instructions.
4. Identify the appropriate next action.

**Success Outcome:** The user understands what to do next.

**Failure Outcome:** The user cannot find or understand the recommended steps.

### Scenario 4: Return to a Previous Screen

**Actor:** User

**Trigger:** The user wants to select a different category or topic.

**Steps:**
1. Select a help category.
2. Open a topic.
3. Select the Back button.
4. Return to the category or homepage.

**Success Outcome:** The user returns to the correct screen and can continue browsing.

**Failure Outcome:** The user cannot find the navigation option or loses their place.

## 4. Requirements

| ID | Requirement | Pattern |
|---|---|---|
| R1 | When a user opens CyberHelp, the system shall display the available help categories. | Event-driven |
| R2 | When a user selects a category, the system shall display the topics in that category. | Event-driven |
| R3 | When a user selects a topic, the system shall display information about the problem. | Event-driven |
| R4 | When a topic is displayed, the system shall show a clear description of the problem. | Event-driven |
| R5 | When warning signs are available for a topic, the system shall display them in a clearly labeled section. | State-driven |
| R6 | When recommended steps are available, the system shall display them under a clearly labeled Recommended Steps heading. | State-driven |
| R7 | The system shall provide navigation options to return to the previous screen or homepage. | Ubiquitous |
| R8 | If a category or topic has no available information, the system shall display a helpful message. | Unwanted behavior |
| R9 | The system shall use simple labels, readable text, and clear navigation. | Ubiquitous |
| R10 | The system shall not request passwords or other sensitive personal information. | Ubiquitous |
| R11 | The system shall organize topics into clearly labeled categories with short descriptions where appropriate. | Ubiquitous |
| R12 | The system shall provide cybersecurity guidance based on reliable sources. | Ubiquitous |

## 5. Acceptance Criteria

| Requirement | Test | Pass Condition |
|---|---|---|
| R1 | Open CyberHelp. | The homepage displays the available categories. |
| R2 | Select a category. | The topics belonging to that category appear. |
| R3 | Select a topic. | The topic information appears. |
| R4 | Open a topic. | A clear problem description is displayed. |
| R5 | Open a topic with warning signs. | The warning signs appear under a clearly labeled heading. |
| R6 | Open a topic with recommended steps. | The recommended steps are easy to locate and read. |
| R7 | Open a topic and select Back. | The user returns to the appropriate previous screen or homepage. |
| R8 | Open a category or topic without available information. | A helpful message explains that information is unavailable. |
| R9 | Browse the website using a keyboard. | Navigation controls can be reached and used, and labels are understandable. |
| R10 | Browse the website. | The website does not request passwords or other sensitive personal information. |
| R11 | Review the homepage and categories. | Categories and topics have clear names, and descriptions are provided where appropriate. |
| R12 | Review the cybersecurity information. | Guidance identifies or links to reliable supporting sources. |

## 6. Constraints & Non-Functional Requirements

### Performance

- Pages should load quickly on a typical internet connection.
- Selecting categories and topics should update the displayed information promptly.
- The initial version should work without a database or complicated backend.

### Security & Privacy

- CyberHelp must not ask users for passwords or other sensitive personal information.
- The initial version should not require users to create accounts.
- Guidance should not encourage users to click suspicious links or download untrusted software.

### Accessibility

- Text should be readable and written in plain language.
- Buttons and links should have clear labels.
- Navigation should be usable with a keyboard.
- Text and background colors should have sufficient contrast.

### Technical Constraints

- The initial version will use HTML, CSS, and JavaScript.
- The prototype should be simple enough to build and test within the course timeframe.
- The website should be compatible with a modern web browser.

### Budget & Timeline

- Development should use existing tools and standard web technologies.
- The initial version should avoid unnecessary hosting, software, and maintenance costs.
- Features should be limited to what can reasonably be completed for the course project.

## 7. Open Questions

| Question | Owner | Status |
|---|---|---|
| Which cybersecurity categories should be included in the first version? | Connor | Resolved: Scams & Phishing, Account Security |
| Which technical support categories should be included in the first version? | Connor | Resolved: Computer Problems |
| How many topics should be included in the first version? | Connor | Resolved: A small collection of common topics |
| Should the initial version include a search bar? | Connor | Resolved: Not required for the first version; consider it for a future update |
| Which sources should be used for cybersecurity information? | Connor | Resolved: Start with FTC and CISA resources |
| Does the prototype make recommended steps easy to find? | Connor | Open until usability testing is completed |
| Can users navigate between screens without confusion? | Connor | Open until usability testing is completed |

## 8. Plan

1. Finalize the initial categories and topics.
2. Build the homepage and category navigation.
3. Add problem descriptions, warning signs, and recommended steps.
4. Add Back buttons and messages for unavailable information.
5. Test the main user scenarios.
6. Ask at least two people to try the prototype and record their feedback.
7. Revise the prototype and specification based on the results.
8. Check the requirements and acceptance criteria before submitting the project.
9. Publish the specification and prepare the final project report.

## 9. Approval

**Specification Owner:** Connor Nease

**Status:** Draft — pending final review and usability testing.

**Approval Date:** To be completed after review.

## Sources

- Federal Trade Commission (FTC): https://consumer.ftc.gov/
- Cybersecurity and Infrastructure Security Agency (CISA): https://www.cisa.gov/secure-our-world
- GitHub Spec Kit: https://github.com/github/spec-kit/blob/main/spec-driven.md
- Microsoft, Spec-Driven Development for AI-Native Engineering: https://developer.microsoft.com/blog/spec-driven-development-ai-native-engineering/
