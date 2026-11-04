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

**Context:** I had already published CyberHelp using GitHub Pages. The design-system page displayed Markdown content, and the web application loaded with working buttons. I needed to figure out what to check next instead of starting the project over.

**AI output and changes:** The guidance focused on verifying the published application, checking the project documentation, and identifying remaining work. I used this guidance to understand that the application could be working even though the design-system document displayed as Markdown. I still needed to finish and organize the supporting project documents.

**Reflection:** This prompt worked well because I explained what I had already tested and what was happening. That made the response more useful than asking a general question about GitHub Pages. I learned that it helps to give the AI specific details about the problem instead of making it guess.

## Example 2: A Prompt That Needed Improvement

**Prompt used:** “How do I make sure this is working?”

**Context:** I was checking whether my CyberHelp web application was functioning correctly on GitHub Pages.

**AI output and changes:** The question did not explain which part of the project I wanted to test or what I had already tried. A more useful prompt would identify the exact page, describe the expected result, and explain what actually happened. For example, I could ask the AI to help me test the homepage, category buttons, topic information, and back-navigation controls one at a time.

**Reflection:** This prompt was too broad because it did not give enough information about what I needed to verify. The response could be more useful if I included the exact page and described the expected behavior. I learned that a specific prompt makes it easier to get steps I can actually follow. I would improve it by explaining what works, what does not work, and what result I expect.

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

Paste the full contents of `docs/design/business-case.md` here.

## Appendix B: Specification

Paste the full contents of `docs/design/specification.md` here.

## Appendix C: Plan

Paste the full contents of `docs/design/plan.md` here.

## Appendix D: Tasks

Paste the full contents of `docs/design/tasks.md` here after creating the file.

## Appendix E: Design System

Paste the full contents of `docs/design/design-system.md` here.
