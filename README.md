# Contribution 1: USACO Guide Open Source Contribution

**Contribution Number:** 1
**Student:** Alston Dsouza
**Repository:** https://github.com/cpinitiative/usaco-guide
**Current Issue:** https://github.com/cpinitiative/usaco-guide/issues/5159
**Status:** Phase II Complete / Phase III In Progress

---

## Why I Chose This Issue

I am contributing to the USACO Guide repository because it matches my experience with JavaScript, React, Next.js, TypeScript, MDX, and frontend development. The project is also well-documented and beginner-friendly, which makes it a good fit for my first open source contribution.

I originally selected issue #3573, "show a message if firebase fails to connect." After investigating it locally, I found that the requested message already existed in the codebase. I contacted the maintainer, and the maintainer confirmed the issue was already resolved and closed it.

After that, I moved to issue #5159, "Contact Form Submission - Suggestion (General - Running Code Online)." I chose this issue because it has a clear scope: update the Running Code Online page by removing online coding platforms that are not suitable for contest use.

---

## Understanding the Issue

### Previous Issue: #3573

Issue #3573 requested a message to help users understand that enabling long polling may help resolve Firebase connection problems.

After setting up the project locally, I found that the requested message already exists in:

```text
src/components/Settings/General.tsx
```

The existing message says:

> "Enable this option ONLY if you encounter issues connecting to Firebase (nothing loads)."

Maintainer **@bqi343** confirmed:

> "yes I think it's fine now"

The issue was then closed as completed.

### Current Issue: #5159

Issue #5159 asks contributors to update the "Running Code Online" page by removing online coding platforms that are not suitable for contest use.

The issue specifically mentions:

* Ideone should be removed because it does not support modern contest standards such as C++17.
* repl.it should be removed because private projects/files are limited unless users pay.

### Expected Behavior

The Running Code Online page should recommend online coding platforms that are more appropriate for contest use.

### Current Behavior Before My Change

Before my change, the page still listed:

* Ideone
* repl.it

These recommendations did not fully match the issue requirements.

### Affected Components

* `content/1_General/Running_Code_Online.mdx`
* Running Code Online page:

  * https://usaco.guide/general/running-code-online?lang=cpp

---

## Reproduction Process

### Environment Setup

I cloned my fork of the USACO Guide repository and installed dependencies using Yarn.

Commands used:

```bash
git clone https://github.com/alstondsouza1/usaco-guide.git
cd usaco-guide
yarn install
yarn dev
```

The application started successfully and was accessible locally at:

```text
http://localhost:3000
```

Yarn displayed some peer dependency warnings, but they did not prevent the site from running.

### Steps to Reproduce Issue #3573

1. Clone the USACO Guide repository.
2. Run `yarn install`.
3. Run `yarn dev`.
4. Open `http://localhost:3000`.
5. Navigate to the Settings page.
6. Locate the "Use Long Polling" option.
7. Verify that the Firebase guidance message already exists.

### Result for Issue #3573

The issue was already implemented. The maintainer confirmed it was resolved and closed the issue.

### Steps to Reproduce Issue #5159

1. Run the USACO Guide project locally.
2. Open:

   ```text
   http://localhost:3000/general/running-code-online?lang=cpp
   ```
3. Review the list of recommended online coding platforms.
4. Confirm that Ideone and repl.it were listed as recommendations.
5. Compare the page with issue #5159, which asks for unsuitable contest-use platforms to be removed.

### Reproduction Evidence

**Current Working Branch:**
https://github.com/alstondsouza1/usaco-guide/tree/update-running-code-online-recommendations

**Current Issue:**
https://github.com/cpinitiative/usaco-guide/issues/5159

**Relevant File:**

```text
content/1_General/Running_Code_Online.mdx
```

**Commit:**

```text
e0a076a0d
```

**Commands Used to Verify Removal:**

```bash
grep -n "Ideone" content/1_General/Running_Code_Online.mdx
grep -n "repl.it" content/1_General/Running_Code_Online.mdx
```

Both commands returned no output, confirming that Ideone and repl.it were removed from the source file.

---

## Solution Approach

### Analysis

For issue #5159, the problem was content-related rather than a complex code bug. The Running Code Online page contained recommendations that were no longer ideal for competitive programming contest use.

The relevant file was:

```text
content/1_General/Running_Code_Online.mdx
```

The maintainer clarified that:

* Ideone should be removed because active contest platforms support C++17 or newer.
* repl.it should be removed because users can only create a limited number of private files/projects.

### Proposed Solution

Update the Running Code Online page by:

1. Removing the Ideone recommendation.
2. Removing the repl.it recommendation.
3. Updating the warning text so it no longer references Ideone specifically.
4. Keeping the change focused only on the relevant MDX content file.

### Implementation Plan

Using the UMPIRE framework:

**Understand:**
The Running Code Online page should only recommend platforms suitable for contest use.

**Match:**
The recommendation list is written directly in `content/1_General/Running_Code_Online.mdx`.

**Plan:**

1. Remove the Ideone section.
2. Remove the repl.it section.
3. Update the contest privacy warning to be general instead of referencing Ideone.
4. Run the site locally and check the page.
5. Verify the source file no longer contains "Ideone" or "repl.it."
6. Commit and push changes to my fork.
7. Open a pull request linked to issue #5159.

**Implement:**
Initial implementation completed in commit `e0a076a0d`.

**Review:**
I checked the diff to confirm the intended file was changed. I also need to make sure unrelated generated files, such as `public/usaco-divisions.json`, are not included in the final pull request.

**Evaluate:**
The page should no longer recommend Ideone or repl.it, and the warning message should give general advice about keeping code private during contests.

---

## Testing Strategy

### Manual Testing

For issue #3573, I manually verified:

* Settings page loads correctly.
* Long polling option is displayed.
* Firebase guidance message is displayed.
* Maintainer confirmed the issue was already resolved.

For issue #5159, I manually verified:

* The source file was updated.
* Ideone was removed from `Running_Code_Online.mdx`.
* repl.it was removed from `Running_Code_Online.mdx`.
* The warning message was updated to no longer reference Ideone directly.

### Command-Line Verification

I ran:

```bash
grep -n "Ideone" content/1_General/Running_Code_Online.mdx
grep -n "repl.it" content/1_General/Running_Code_Online.mdx
```

Both returned no output.

### Remaining Testing

Before opening the pull request, I will verify the page renders correctly locally and that only intended files are included in the final diff.

---

## Implementation Notes

### Week 1 Progress

* Created the Contribution README repository.
* Selected issue #3573.
* Forked the USACO Guide repository.
* Commented on the issue.
* Set up the local development environment.
* Began investigating the codebase.

### Week 2 Progress

Successfully:

* Ran the USACO Guide project locally.
* Investigated issue #3573.
* Located the existing Firebase guidance message.
* Asked the maintainer for clarification.
* Received confirmation that issue #3573 was already resolved.
* Observed the maintainer close issue #3573.
* Selected a new active issue: #5159.
* Commented on issue #5159 to express interest.
* Created a new branch:

  ```text
  update-running-code-online-recommendations
  ```
* Located the relevant file:

  ```text
  content/1_General/Running_Code_Online.mdx
  ```
* Removed Ideone and repl.it recommendations.
* Updated the contest privacy warning message.
* Committed and pushed the change.

### Code Changes

**Files modified:**

```text
content/1_General/Running_Code_Online.mdx
```

**Branch:**

```text
update-running-code-online-recommendations
```

**Commit:**

```text
e0a076a0d
```

### Outcome So Far

Issue #3573 required no code change because it was already implemented and closed by the maintainer.

Issue #5159 is now the active contribution. The initial code/content change has been committed and pushed. The next step is to open a pull request.

---

## Pull Request

**PR Link:** TBD

**Status:** Ready to open pull request

**Planned PR Summary:**

* Removes Ideone from the Running Code Online recommendations.
* Removes repl.it from the Running Code Online recommendations.
* Updates the contest privacy warning so it is no longer tied to Ideone.

**Related Issue:**

```text
Closes #5159
```

---

## Learnings & Reflections

### Technical Skills Gained

* Set up and ran a large Next.js and TypeScript project locally.
* Navigated an unfamiliar open source codebase.
* Located content files in an MDX-based documentation site.
* Used Git branches, commits, and pushes for open source workflow.
* Practiced verifying whether an issue still exists before implementing a fix.
* Communicated with project maintainers.

### Challenges Overcome

The first issue I selected was already implemented even though it remained open. I learned that this can happen in open source projects and that it is important to investigate before making code changes.

For the second issue, the main challenge was understanding where the page content lived and making a small, focused change without touching unrelated files.

### What I'd Do Differently Next Time

I would verify the current state of an issue earlier before committing to it. I would also check `git status` carefully before committing to avoid accidentally including unrelated generated files.

### Key Lesson

A good open source contribution is not only about writing code. It also includes reproducing issues, checking existing implementation, communicating clearly with maintainers, keeping changes focused, and documenting the process.

---

## Resources Used

* https://github.com/cpinitiative/usaco-guide/issues/3573
* https://github.com/cpinitiative/usaco-guide/issues/5159
* https://github.com/cpinitiative/usaco-guide
* USACO Guide README
* USACO Guide source code
* CodePath AI301 Phase I Instructions
* CodePath AI301 Phase II Instructions
* First Contributions Tutorial
* Claude Code setup through CodePath/Anthropic
