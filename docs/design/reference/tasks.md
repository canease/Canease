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