# CyberHelp — Research

## 1. Competitive Analysis

I looked at three websites that provide cybersecurity information or support: the FTC, CISA, and Norton.

### Competitor 1: Federal Trade Commission (FTC)

**What it does:**

* Provides information about scams and cybersecurity problems.
* Gives users steps to take when something goes wrong.
* Covers topics such as phishing, hacked accounts, and tech support scams.

**Interaction flow:**

1. User searches for a problem.
2. User opens an article.
3. User reads information about the problem.
4. User follows the recommended steps.

**What CyberHelp can learn from it:**

* Information should include clear steps.
* Users should be able to quickly understand what to do next.
* CyberHelp can organize problems into categories.

### Competitor 2: CISA

**What it does:**

* Provides cybersecurity advice for the general public.
* Covers topics such as software updates, passwords, and online safety.
* Uses simple tips and guides.

**Interaction flow:**

1. User visits the website.
2. User chooses a security topic.
3. User reads the advice.
4. User follows the recommended action.

**What CyberHelp can learn from it:**

* Keep information simple.
* Use topics that people can understand.
* Give users practical actions.

### Competitor 3: Norton

**What it does:**

* Provides cybersecurity information and technical support.
* Has search and different help areas.
* Provides information about scams, malware, passwords, and other security problems.

**Interaction flow:**

1. User visits the support page.
2. User searches for a problem or chooses a help topic.
3. User reads the instructions.
4. User follows the recommended steps.

**What CyberHelp can learn from it:**

* Search can be useful.
* There are many different types of cybersecurity problems.
* CyberHelp should avoid giving users too much information at once.

### Competitive Analysis Summary

The three competitors provide:

* Categories or topics.
* Search or browsing.
* Explanations of problems.
* Warning signs.
* Recommended steps.

CyberHelp can focus on making this information simpler and easier for beginners to understand.

---

# 2. User Interviews / Survey

I asked two people about how they currently deal with cybersecurity and computer problems.

### Questions

**Question 1 — Current behavior**

When you have a cybersecurity or computer problem, what do you normally do to find help?

**Question 2 — Pain points**

What is the most difficult or frustrating part about finding help?

**Question 3 — Desired features**

What would you want a website like CyberHelp to have that would make finding help easier?

### Person 1 — Layne

**Question 1 — Current behavior**

Usually I just Google it or ask somebody I know who is better with computers. Sometimes I'll watch a YouTube video if I can't figure it out.

**Question 2 — Pain points**

A lot of the websites use words I don't really understand. Sometimes there are a bunch of different answers and I don't know which one to trust.

**Question 3 — Desired features**

I'd want it to be simple and tell me what the problem probably is and what I should do. It would also be nice if I didn't have to read a huge article.

### Person 2 — Devin

**Question 1 — Current behavior**

I usually search online or ask a friend or family member. If it's something with my computer, sometimes I'll just take it to somebody who knows more about computers.

**Question 2 — Pain points**

It's hard to know if the information online is actually right. Some websites make things sound more complicated than they need to be.

**Question 3 — Desired features**

I'd like to be able to pick what kind of problem I'm having and then see the answer. Having steps to follow would be helpful too.

### User Research Findings

**How people currently find help:**

People usually search online, watch videos, or ask friends and family.

**Main problems people have:**

* Technical information can be confusing.
* There can be too many different answers.
* It can be hard to know which information to trust.

**Features people want:**

* Simple explanations.
* Organized topics.
* Clear steps to follow.

**Changes this suggests for CyberHelp:**

CyberHelp should keep information simple, organize problems into categories, and provide clear steps.

---

# 3. Technical Feasibility Check

CyberHelp is technically feasible because the first version will be a simple website.

### Technology

The application can use:

* HTML for the website structure.
* CSS for the design.
* JavaScript for simple interactions.

### Hosting

The website can be hosted using GitHub Pages.

### Features That Are Feasible

The following features should be simple enough to build:

* Category buttons.
* Topic buttons.
* Information pages.
* Back buttons.
* Basic search if needed.
* Responsive design.
* Basic accessibility features.

### Features Not Needed

The first version does not need:

* User accounts.
* A database.
* Live cybersecurity scanning.
* Automatic malware detection.
* Payments.
* Passwords.
* Remote computer access.

### Technical Conclusion

CyberHelp can be built as a simple website using HTML, CSS, and JavaScript. Keeping the first version small will make it easier to complete within the course timeframe.

---

# 4. Summary of Research Findings

The research shows that there are already many websites with cybersecurity information. CyberHelp can focus on making this information easier for beginners to find and understand.

The research supports:

* Using categories to organize information.
* Keeping explanations short and simple.
* Showing warning signs.
* Providing recommended steps.
* Making navigation simple.
* Avoiding unnecessary features.
* Using reliable sources.

The user research also suggests that users want simple information and clear steps instead of long or complicated explanations.

---

# 5. Prototype

## Prototype Goal

The prototype will test the main CyberHelp interaction:

**Home → Category → Topic → Problem Information → Recommended Steps**

The prototype only needs to show how a user would move through the application.

## Prototype Screens

### Screen 1 — Home

The home page will include:

**CyberHelp**

"Find help for common cybersecurity and technical problems."

Categories:

* Scams & Phishing
* Account Security
* Computer Problems
* Online Safety

### Screen 2 — Category

**Scams & Phishing**

* Phishing Emails
* Scam Text Messages
* Tech Support Scams

The user selects a topic.

### Screen 3 — Topic

**Phishing Emails**

**What is it?**

A phishing email is a message designed to trick you into clicking a link or giving away personal information.

**Warning Signs:**

* Unexpected message
* Urgent request
* Suspicious link
* Request for personal information

### Screen 4 — Recommended Steps

**What should I do?**

1. Do not click suspicious links.
2. Do not provide personal information.
3. Contact the company using a website or phone number you know is real.
4. Report the message if necessary.

The page will also have a **Back** button.

---

# 6. Prototype Evaluation

The prototype was tested by me and two other people. The main goal was to see if users could find a cybersecurity problem and understand the recommended steps.

## Observation 1

**Person:** Layne

**Task:** Find information about a phishing email.

**What happened:**

The user was able to find the "Scams & Phishing" category and then select "Phishing Emails."

**Problem noticed:**

The user was not sure what category to choose at first.

**Possible change:**

Make the category names more specific and add a short description under each category.

---

## Observation 2

**Person:** Devin

**Task:** Find the recommended steps for a cybersecurity problem.

**What happened:**

The user found the phishing email page but had to scroll to find the recommended steps.

**Problem noticed:**

The recommended steps were not easy to find.

**Possible change:**

Put "Recommended Steps" in a clear section or heading.

---

## My Observation

**Task tested:**

Find a cybersecurity problem and read the recommended steps.

**What happened:**

I was able to move from the home page to a category, then to a topic, and finally to the recommended steps.

**Problem noticed:**

The prototype could use clearer navigation between the different pages.

**Possible change:**

Add clear Back buttons to the category and topic pages.

---

# 7. Prototype Findings

### What worked well?

* Users were able to select a category and find a topic.
* The basic category → topic → information flow was easy to understand.

### What was confusing?

* Some category names were not immediately clear.
* The recommended steps were not always easy to find.

### What should be changed?

* Make category names clearer.
* Make recommended steps more noticeable.
* Add clearer navigation buttons.

### Changes to Make

Based on the prototype testing, CyberHelp should:

* Use simple and descriptive category names.
* Put recommended steps under a clearly labeled heading.
* Add clear Back buttons to make navigation easier.

---

# 8. Prototype Images

The prototype will include screenshots of the main screens:

* `HomePage.jpeg`
* `Category.jpeg`
* `Problem.jpeg`
* `Problemexplained.jpeg`
* `helpchecklist.jpeg`

These images will show the main interaction flow of CyberHelp.

---

# 9. Research Conclusion

The research supports the original idea for CyberHelp. Existing cybersecurity websites provide useful information, but CyberHelp can focus on making that information easier for beginners to find and understand.

The prototype testing showed that the basic category → topic → information flow works, but the categories and navigation could be clearer.

The specification will be updated based on the research and prototype findings.
