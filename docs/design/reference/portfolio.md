# CyberHelp Portfolio

**Author:** Connor Nease  
**Project:** CyberHelp  
**Course:** CSCI-490 Client Server Web Programming  
**Date:** October 2026

# Part 1: Traceability Audit

The traceability audit connects the original business case to the requirements, acceptance tests, design decisions, and development tasks. This helps make sure the work being done supports the original goal of CyberHelp.

| Business Case Benefit | Requirement | Acceptance Test | ADR | Task |
|---|---|---|---|---|
| Faster access to cybersecurity information | R1: The homepage displays available categories. | Open the application and verify that the categories are displayed. | ADR-02: Organize information by categories and topics. | T1: Build and verify the homepage. |
| Better organization of technical information | R2: Selecting a category displays its topics. | Select a category and verify that its topics appear. | ADR-02: Organize information by categories and topics. | T2: Build and verify category navigation. |
| Improved cybersecurity awareness | R6: Recommended steps appear under a clearly labeled section. | Open a topic and verify that recommended steps appear under the heading “Recommended Steps.” | ADR-03: Use clearly labeled sections for topic information. | T3: Build and verify topic information. |

**Traceability note:** The ADR and task IDs above are proposed references for organizing the project. The ADR and tasks documents must be created and kept consistent with these references before the audit can be considered fully verified.

# Part 2: AI Collaboration Evidence

## Example 1: A Prompt That Helped

**Prompt used:**

“Help me verify my GitHub Pages project. Design-system document result: displays Markdown content. Web application result: CyberHelp loads and buttons work. Give me the specific next steps.”

**Context:** I had checked my published project and confirmed that the web application loaded and its buttons worked. I wanted to know what I should do next.

**AI output and changes:** The response gave me next steps based on the results I reported. I used the guidance to focus on finishing the project documentation and checking the remaining requirements instead of rebuilding the application.

**Reflection:** This prompt worked well because I explained what I had already tested and what I found. That helped make the response specific to my project. I learned that including the results of my own checks makes it easier to get useful next steps.

## Example 2: A Prompt That Needed Improvement

**Prompt used:**

“How do I make sure this is working?”

**Context:** I was checking whether my CyberHelp web application was functioning correctly on GitHub Pages.

**AI output and changes:** The question was broad and did not say which part of the application I wanted to test. A more useful prompt would name the feature and describe what should happen—for example, asking how to test whether selecting a category displays its topics. I would then compare the guidance with what I observed on the published site.

**Reflection:** This prompt needed more detail because “this” could refer to several parts of the project. I learned that I should describe the feature I am testing and what I expect to happen. That would make the response easier to follow and the results easier to verify.

# Part 3: Document Reflection

## Document That Paid Off the Most

The specification was one of the most useful documents for CyberHelp because it explained what the application needed to do. It identified the intended users, the project scope, and the requirements for categories, topics, warning signs, recommended steps, navigation, privacy, and reliable sources. Having those requirements written down gave me something to check against while working on the application. It also helped keep the project focused on providing simple cybersecurity information instead of adding features that were outside the original scope.

## Document That Needed the Most Improvement

The plan needed the most improvement because it still needed more specific decisions, tasks, and a clear order for completing the work. A plan is more useful when it explains what needs to happen first, what depends on other work, and how progress will be checked. The project also needed an actual tasks document and architecture decision records instead of only proposed examples. Finishing these documents would make it easier to track the work and show how the requirements connect to the implementation.

# Appendix

The appendix should contain the current full versions of the project documents in the following order:

1. Business Case
2. Specification
3. Plan
4. Tasks
5. Design System

**Appendix completion note:** Replace the placeholders below with the complete contents of each current GitHub document. The portfolio appendix is not complete until the full documents are included.

## Appendix A: Business Case

# Business Case — CyberHelp

## 1. Problem / Opportunity
Many people struggle to find reliable and easy-to-understand information when dealing with common cybersecurity and technical problems. A centralized web application could make this information easier to find and understand without requiring users to search through multiple websites.

## 2. Proposed Solution
CyberHelp would provide users with a simple collection of common cybersecurity and technical support topics. Users could select a topic to view information about the problem, common warning signs, and recommended steps for addressing it. The application would organize the information in one location so users could quickly find help without searching through multiple sources.

## 3. Options Considered

| Option | Description | Pros | Cons |
|--------|-------------|------|------|
| Option A | Users search for cybersecurity problems using keywords. | Fast and flexible for experienced users. | Users may not know what to search for. |
| Option B (recommended) | Users browse organized categories and select a topic for detailed information. | Simple, organized, and easy for beginners. | Information must be organized into categories. |

## 4. Feasibility

| Type | Assessment |
|------|------------|
| Operational — will people actually use/support this? | The application would be easy to understand and useful for people looking for help with common cybersecurity problems. |
| Technical — can we build it with what we have/can get? | The application can be developed using standard web technologies and a small collection of simulated information. |
| Economic — does the payoff justify the cost? | Development costs would be relatively low because the prototype can use existing development tools and services. |
| Schedule — can it be done in a useful timeframe? | A basic version can be developed within the course timeframe because the application has a limited number of features. |

## 5. Costs & Benefits

**Costs** (one-time + ongoing):

| Item | One-time | Ongoing/year |
|------|----------|----------------|
| Development | $1,000 | $0 |
| Domain/hosting | $25 | $25 |
| Maintenance | $0 | $200 |
| **Total** | **$1,025** | **$225** |

**Benefits** (tangible + intangible):

| Benefit | Tangible ($/time saved)? | Notes |
|---------|-----------------------------|-------|
| Faster access to information | 2 hours/week saved | Users spend less time searching for answers. |
| Better organization | 1 hour/week saved | Information is available in one location. |
| Improved cybersecurity awareness | Intangible | Users can learn how to recognize common threats. |

**Payback period:** Approximately 6 months
**ROI:** Approximately 95%

*(See Toolkit Part C — Financial Analysis Tools document for payback, ROI, and present value formulas.)*

## 6. Priority & Urgency
Cybersecurity information is increasingly important as individuals and organizations face more online threats. Without a centralized resource, users may continue relying on random search results or outdated information when trying to solve common security problems.

## 7. Recommendation
I recommend Option B because it provides a simple and organized way for users to find cybersecurity information, and I recommend moving forward with development of the application.
## 8. Approval

| Role | Name | Date | Decision |
|------|------|------|----------|
| Sponsor | John Doe | September 7, 2026 | Go |
---

### Primary sources
- *Systems Analysis and Design*, 10th ed. (Cengage, 2017) — Ch. 2 "Analyzing the Business Case" and Toolkit Part C "Financial Analysis Tools"


## Appendix B: Specification

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

## Appendix C: Plan

# Plan - CyberHelp

## 1. Approach Summary

CyberHelp is a simple web application that organizes common cybersecurity and technical problems into categories and topics. Users can select a category, open a topic, read the problem description and warning signs, and find recommended steps. The application uses HTML, CSS, and JavaScript and is published through GitHub Pages. The first version focuses on simple navigation, readable information, and reliable cybersecurity resources rather than accounts, databases, or live technical support.

## 1.5 Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend/DB:** None required for the initial version
- **Hosting:** GitHub Pages
- **Other services/APIs:** Links to reliable external resources, including the FTC and CISA

## 2. Key Decisions (ADRs)

| ADR # | Decision | Traces to (R#) | Alternatives considered | Why this one |
|---|---|---|---|---|
| ADR-01 | Use HTML, CSS, and JavaScript for the initial application. | R1, R2, R3, R7, R9 | Use a frontend framework or add a backend. | The project is a small informational website, so standard web technologies keep it simple and easy to maintain. |
| ADR-02 | Organize help through categories and topics instead of requiring keyword search. | R1, R2, R3, R11 | Start with a search-first interface. | Browsing categories gives beginners a clear starting point even when they do not know the right technical terms. |
| ADR-03 | Use clearly labeled topic sections for descriptions, warning signs, and recommended steps. | R4, R5, R6 | Put all topic information into one long block of text. | Separate sections make the information easier to scan and help users find what to do next. |
| ADR-04 | Use reliable public cybersecurity sources, including the FTC and CISA. | R10, R12 | Write guidance without linking to supporting sources. | Reliable sources help users find trustworthy information, and the application should not request passwords or sensitive personal information. |
| ADR-05 | Publish the initial version using GitHub Pages without a database or user accounts. | R1, R9, R10 | Add a backend, database, and account system. | The application provides informational content, so a static site meets the initial needs without collecting user data or adding unnecessary complexity. |

## 3. Components / Building Blocks

| Component | Purpose | Related requirements |
|---|---|---|
| Homepage | Displays the available help categories. | R1, R9, R11 |
| Category navigation | Displays topics within a selected category. | R2, R7, R11 |
| Topic content | Shows the problem description, warning signs, and recommended steps. | R3, R4, R5, R6 |
| Navigation controls | Allow users to return to the previous screen or homepage. | R7 |
| Unavailable-information message | Explains when information is not available. | R8 |
| Source links | Connect users to reliable cybersecurity guidance. | R10, R12 |
| Shared styles and layout | Keep the site readable and consistent. | R9 |

## 4. Dependencies & Assumptions

- Development uses HTML, CSS, and JavaScript.
- GitHub Pages is used to publish the website.
- Users have a modern web browser and an internet connection.
- CyberHelp begins with a limited set of common topics.
- FTC and CISA resources provide starting points for cybersecurity guidance.
- The site does not need a database, login system, or live support for the initial version.
- External source links and guidance should be checked for accuracy.

## 5. Risks

| Risk | Likelihood | Impact | Mitigation | Owner |
|---|---|---|---|---|
| Users cannot tell which category fits their problem. | Medium | Medium | Use clear category names and short descriptions, then test with users. | Connor Nease |
| Users have trouble finding recommended steps. | Medium | High | Use a clearly labeled Recommended Steps heading and test topic pages. | Connor Nease |
| Cybersecurity information becomes outdated. | Medium | High | Use reliable sources and review source links and guidance. | Connor Nease |
| Users cannot easily return to a previous screen. | Medium | Medium | Provide clear Back or Return to Categories controls and test navigation. | Connor Nease |
| Published pages do not work as expected. | Low | Medium | Test the published GitHub Pages site and its main navigation flows. | Connor Nease |

## 6. Sequencing

1. Confirm the initial categories and topics.
2. Build and check the homepage and category navigation.
3. Add topic descriptions, warning signs, and recommended steps.
4. Add and test navigation controls and unavailable-information messages.
5. Verify source links and check that no passwords or sensitive information are requested.
6. Test the main user scenarios and acceptance criteria in the specification.
7. Ask users to try the prototype, record confusing areas, and make improvements.
8. Test the published version on GitHub Pages and update the documentation to match the final application.

## 7. Review & Approval

- **Reviewer:** Connor Nease
- **Date:** Enter the date you review and finalize this plan.
- **Approved?:** Pending review

**Gate:** Create and maintain `tasks.md` after the Plan decisions and sequencing have been reviewed. Keep task IDs connected to the requirements above.

## Appendix D: Tasks

# CyberHelp - Tasks

These tasks connect the CyberHelp specification requirements to implementation and testing. Task IDs are used in the portfolio traceability audit.

## T1: Build and Verify the Homepage

**Related requirements:** R1, R9, R11  
**Purpose:** Make it easy for users to find the right starting category.

**Work:**
- Display the available help categories on the homepage.
- Use clear category names and short descriptions where appropriate.
- Keep labels and navigation understandable.

**Acceptance check:** Open CyberHelp and confirm that the homepage displays clearly labeled categories.

**Status:** Complete

## T2: Build and Verify Category Navigation

**Related requirements:** R2, R7, R11  
**Purpose:** Help users browse topics and move between screens.

**Work:**
- Display the topics belonging to each category.
- Provide clear navigation back to the appropriate previous screen or homepage.
- Test category and topic navigation.

**Acceptance check:** Select a category, open a topic, and return to the appropriate screen.

**Status:** Complete

## T3: Build and Verify Topic Information

**Related requirements:** R3, R4, R5, R6  
**Purpose:** Make problem information and recommended actions easy to understand.

**Work:**
- Display a clear description for each topic.
- Include warning signs when available.
- Place recommended actions under a clearly labeled Recommended Steps heading.

**Acceptance check:** Open a topic and confirm its description, warning signs when available, and recommended steps when available are easy to find.

**Status:** Complete

## T4: Handle Missing Information

**Related requirements:** R8  
**Purpose:** Avoid leaving users confused when information is unavailable.

**Work:**
- Check how the application behaves when a category or topic has no information.
- Display a helpful message where applicable.

**Acceptance check:** Verify that an unavailable category or topic produces a helpful message.

**Status:** Complete

## T5: Verify Privacy and Reliable Sources

**Related requirements:** R10, R12  
**Purpose:** Keep the guidance responsible and help users find trustworthy information.

**Work:**
- Confirm that the application does not ask users for passwords or sensitive personal information.
- Check cybersecurity guidance and links to reliable sources such as the FTC and CISA.

**Acceptance check:** Review the application for requests for sensitive information and verify that relevant cybersecurity guidance identifies or links to reliable sources.

**Status:** Complete

## T6: Test and Refine the Application

**Related requirements:** R1–R12, as applicable to each test  
**Purpose:** Check the main user scenarios and fix usability problems.

**Work:**
- Test opening the homepage, selecting a category, opening a topic, and returning to a previous screen.
- Check that descriptions, warning signs, and recommended steps are understandable.
- Record feedback from usability testing and make appropriate improvements.
- Test the published GitHub Pages version.

**Acceptance check:** Record the test results, identify any failed checks, and document fixes or remaining limitations.

**Status:** Complete

## Appendix E: Design System

# CyberHelp Design System

## 1. Overview

CyberHelp is a simple web application that helps users find information about common cybersecurity and technical problems. The design focuses on being easy to understand, organized, and accessible to people with different levels of technical experience.

The goal is to help users find useful information and recommended steps without having to search through multiple websites.

## 2. Design Goals

- Keep the website simple and easy to navigate.
- Use clear language that beginners can understand.
- Organize information into categories and topics.
- Make recommended steps easy to find and follow.
- Keep the appearance consistent across all pages.
- Make the website usable on both desktop computers and mobile devices.

## 3. Color Palette

- **Primary color:** Dark blue (`#1D3557`) for the main header, navigation, and important elements.
- **Secondary color:** Blue (`#457B9D`) for links and secondary buttons.
- **Background color:** Light gray (`#F5F7FA`) for the main page background.
- **Card color:** White (`#FFFFFF`) for content sections and topic cards.
- **Text color:** Dark gray (`#263238`) for normal text.
- **Success color:** Green (`#2E7D32`) for positive messages and helpful outcomes.
- **Warning color:** Orange (`#ED8B00`) for security warnings and caution messages.
- **Border color:** Light gray (`#D9E0E7`) for separating sections and cards.

## 4. Typography

- **Font family:** Arial or a similar sans-serif font.
- **Main heading:** Large, bold text that clearly identifies the page.
- **Section headings:** Medium-sized bold text used to organize information.
- **Body text:** Regular text with enough spacing to make reading comfortable.
- **Instructions:** Numbered lists for steps users should follow.
- **Links:** Clearly distinguishable from normal text.

## 5. Layout and Spacing

- Use a consistent header at the top of the page.
- Place the main content in a centered container with a readable maximum width.
- Use cards to separate categories and individual topics.
- Keep consistent spacing between headings, paragraphs, buttons, and cards.
- Use a simple layout that does not overwhelm users with too much information at once.

## 6. Components

### Header

The header displays the CyberHelp name and provides a consistent starting point for navigation.

### Category Cards

Category cards help users browse common types of problems, such as:

- Scams and Phishing
- Account Security
- Computer Problems

Each card should have a clear title and a short description.

### Topic Links

Topic links allow users to select a specific problem within a category. Names should describe the problem in plain language.

### Information Sections

Problem pages should organize information into clear sections:

- Problem Overview
- Warning Signs
- Recommended Steps

### Buttons

Buttons should use clear labels such as **View Topic**, **Back**, or **Return to Categories**. Buttons should look consistent throughout the application.

### Warning Messages

Warnings should stand out from regular information and explain what users should watch for or avoid. Important warnings should include text, not rely on color alone.

## 7. Navigation

Users should be able to move from the homepage to a category, from a category to a topic, and back to previous pages.

Navigation should be predictable and should not require users to know technical terms. Users should always have a clear way to return to the previous section or the homepage.

## 8. Accessibility

- Use readable text sizes and sufficient contrast.
- Use descriptive labels for buttons and links.
- Organize content with headings in a logical order.
- Make sure interactive elements can be used with a keyboard.
- Do not communicate warnings through color alone.
- Keep instructions short and easy to follow.
- Use responsive layouts so content remains usable on smaller screens.

## 9. Responsive Design

The website should work on desktop computers, tablets, and mobile phones. On smaller screens, cards should stack vertically, text should remain readable, and buttons should be easy to select.

## 10. Content Guidelines

CyberHelp should use simple, direct language. Avoid unnecessary technical terms, and explain unfamiliar terms when they are needed.

Cybersecurity instructions should be presented in a clear order. Information should focus on helping users recognize a problem, understand the risks, and take reasonable next steps.

## 11. Consistency Rules

All pages should use the same colors, fonts, spacing, card styles, and button styles. Headings should follow a consistent hierarchy, and similar actions should use the same labels across the website.

The design should prioritize clarity and usability over decorative effects.

## 12. Future Improvements

Possible future improvements include adding a search feature, improving mobile navigation, adding more cybersecurity topics, and reviewing accessibility with user feedback.