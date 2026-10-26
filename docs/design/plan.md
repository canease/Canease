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