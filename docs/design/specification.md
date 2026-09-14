# CyberHelp — Specification

## 1. Problem & Intent

**Who is this for?**

People who need help with common cybersecurity or technical problems.

**What problem does it solve?**

People may have trouble finding simple and reliable information about cybersecurity problems because they have to search through many different websites.

**What does success look like?**

* Users can find a category that matches their problem.
* Users can find information about their problem.
* Users can understand the recommended steps.
* Users can move through the website without getting confused.

---

## 2. Scope

**In scope**

* Cybersecurity and technical support categories.
* Topics within each category.
* Basic information about each problem.
* Common warning signs.
* Recommended steps.
* Simple navigation between pages.

**Out of scope**

* Live technical support.
* Automatically fixing problems.
* Malware removal.
* Live cybersecurity monitoring.
* User accounts.
* Payments.
* Collecting passwords or other sensitive information.

---

## 3. User Scenarios

### Scenario 1: Find a Help Topic

* **Actor:** User
* **Trigger:** User has a cybersecurity or technical problem.
* **Steps:**

  1. Open CyberHelp.
  2. Look at the categories.
  3. Select a category.
  4. Select a topic.
* **Success outcome:** User finds information about their problem.
* **Failure outcome:** User cannot find a category or topic that matches their problem.

### Scenario 2: Understand a Problem

* **Actor:** User
* **Trigger:** User selects a help topic.
* **Steps:**

  1. Read the problem description.
  2. Look at the warning signs.
  3. Decide if the information matches their problem.
* **Success outcome:** User understands the problem.
* **Failure outcome:** Information is confusing or does not help the user.

### Scenario 3: Find Recommended Steps

* **Actor:** User
* **Trigger:** User wants to know what to do about a problem.
* **Steps:**

  1. Open a topic.
  2. Read the recommended steps.
  3. Follow the steps that apply to the problem.
* **Success outcome:** User understands what they should do next.
* **Failure outcome:** User does not understand the recommended steps.

---

## 4. Requirements

| ID  | Requirement                                                                                                | Pattern           |
| --- | ---------------------------------------------------------------------------------------------------------- | ----------------- |
| R1  | When a user opens CyberHelp, the system shall show the available categories.                               | Event             |
| R2  | When a user selects a category, the system shall show the topics in that category.                         | Event             |
| R3  | When a user selects a topic, the system shall show information about the problem.                          | Event             |
| R4  | When a topic is shown, the system shall show a description of the problem.                                 | Event             |
| R5  | When available, the system shall show common warning signs.                                                | Event             |
| R6  | When available, the system shall show recommended steps.                                                   | Event             |
| R7  | The system shall provide a way for the user to return to the previous page.                                | Event             |
| R8  | If a category has no topics, the system shall show a message explaining that information is not available. | Unwanted behavior |
| R9  | The system shall use simple labels and navigation.                                                         | Ubiquitous        |
| R10 | The system shall not ask users for passwords or other sensitive information.                               | Ubiquitous        |

---

## 5. Acceptance Criteria

| Requirement | Test                                 | Pass Condition                                     |
| ----------- | ------------------------------------ | -------------------------------------------------- |
| R1          | Open CyberHelp.                      | Categories are shown.                              |
| R2          | Select a category.                   | Topics are shown.                                  |
| R3          | Select a topic.                      | Problem information is shown.                      |
| R4          | Open a topic.                        | A problem description is shown.                    |
| R5          | Open a topic with warning signs.     | Warning signs are easy to find.                    |
| R6          | Open a topic with recommended steps. | Recommended steps are easy to find.                |
| R7          | Select the back option.              | User returns to the previous page.                 |
| R8          | Select an empty category.            | A clear message is shown.                          |
| R9          | Browse the website.                  | Labels and navigation are easy to understand.      |
| R10         | Browse CyberHelp.                    | No password or sensitive information is requested. |

---

## 6. Constraints & Non-Functional Requirements

**Performance**

* Pages should load quickly.
* The website should respond when users select categories and topics.

**Security & Privacy**

* CyberHelp should not ask users for passwords.
* CyberHelp should not require sensitive personal information.

**Accessibility**

* Text should be easy to read.
* Buttons and links should be clearly labeled.
* The website should be usable with a keyboard.

**Budget & Timeline**

* The project should use standard web technologies.
* The project should be simple enough to complete within the course timeframe.

---

## 7. Open Questions

| Question                                              | Owner  | Status |
| ----------------------------------------------------- | ------ | ------ |
| What cybersecurity categories should be included?     | Connor | Open   |
| What technical support categories should be included? | Connor | Open   |
| How many topics should be included?                   | Connor | Open   |
| Should the website have a search bar?                 | Connor | Open   |
| What sources should be used for the information?      | Connor | Open   |

---

## 8. Plan

After the specification is approved, the next steps will be:

* Decide on the categories and topics.
* Create the basic website pages.
* Add the cybersecurity information.
* Add navigation between pages.
* Test the main user scenarios.
* Make changes based on user feedback.

---

## Sources

* [GitHub Spec Kit — Spec-Driven Development](https://github.com/github/spec-kit/blob/main/spec-driven.md)
* [Microsoft — Spec-Driven Development for AI-Native Engineering](https://developer.microsoft.com/blog/spec-driven-development-ai-native-engineering/)
