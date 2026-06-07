# Contribution 1: Remove Ideone and repl.it from Running Code Online Recommendations

**Contribution Number:** 1
**Student:** Alston Dsouza
**Issue:** https://github.com/cpinitiative/usaco-guide/issues/5159
**Status:** Phase IV Complete (Merged)

---

## Why I Chose This Issue

I chose this issue because it matched my experience with JavaScript, TypeScript, React, Next.js, and frontend-focused projects. The USACO Guide repository is well documented and beginner friendly, making it a good project for my first open-source contribution.

I was also interested in learning the complete open-source workflow, including investigating issues, communicating with maintainers, creating pull requests, responding to automated checks, and getting code merged into a production repository.

---

## Understanding the Issue

### Problem Description

The Running Code Online page contained recommendations for Ideone and repl.it. The issue reported that these platforms were no longer ideal recommendations for competitive programming contests.

### Expected Behavior

The page should recommend platforms that support modern contest environments and allow private work without significant restrictions.

### Current Behavior

The page still recommended Ideone and repl.it.

### Affected Components

* content/1_General/Running_Code_Online.mdx
* Running Code Online documentation page

---

## Reproduction Process

### Environment Setup

```bash
git clone https://github.com/alstondsouza1/usaco-guide.git
cd usaco-guide
yarn install
yarn dev
```

### Steps to Reproduce

1. Run the USACO Guide project locally.
2. Navigate to `/general/running-code-online`.
3. Review the recommended platforms.
4. Observe Ideone and repl.it listed on the page.

### Reproduction Evidence

Commit:
https://github.com/alstondsouza1/usaco-guide/commit/e0a076a0d

Finding:
Ideone and repl.it were still listed despite maintainer guidance that they should be removed.

---

## Solution Approach

### Analysis

The issue was documentation-related. The recommendations were stored directly inside the MDX file that generates the page.

### Proposed Solution

1. Remove Ideone.
2. Remove repl.it.
3. Update the warning text to be platform-agnostic.

### Implementation Plan

* Locate recommendation list.
* Remove outdated platforms.
* Verify documentation renders correctly.
* Submit pull request.

### Implement

Branch:
https://github.com/alstondsouza1/usaco-guide/tree/update-running-code-online-recommendations

PR:
https://github.com/cpinitiative/usaco-guide/pull/6238

### Evaluate

Confirmed Ideone and repl.it no longer appear on the page.

---

## Testing Strategy

### Manual Testing

* Verified page builds locally.
* Verified Ideone removed.
* Verified repl.it removed.
* Verified warning text renders correctly.

---

## Implementation Notes

### Week 1 Progress

* Selected issue.
* Forked repository.
* Set up development environment.

### Week 2 Progress

* Located affected file.
* Implemented changes.
* Opened PR.

### Week 3 Progress

* Passed automated checks.
* Received maintainer review.
* PR approved and merged.

### Code Changes

Files Modified:

```text
content/1_General/Running_Code_Online.mdx
```

Commit:

```text
e0a076a0d
```

---

## Pull Request

PR:
https://github.com/cpinitiative/usaco-guide/pull/6238

Status:
Merged ✅

Maintainer Feedback:

* Approved by @bqi343
* Merged into master

---

## Learnings & Reflections

### Technical Skills Gained

* Git branching and pull requests
* MDX documentation editing
* Open source workflow
* Maintainer communication

### Challenges Overcome

My original issue (#3573) had already been implemented despite remaining open. I learned how to investigate issues before implementing changes and successfully pivoted to another contribution.

---

## Resources Used

* Issue #3573
* Issue #5159
* PR #6238
* USACO Guide source code
* CodePath AI301 materials

---

# Contribution 2: Expand USACO FAQ

**Contribution Number:** 2
**Student:** Alston Dsouza
**Issue:** https://github.com/cpinitiative/usaco-guide/issues/3384
**Status:** Phase II In Progress

---

## Why I Chose This Issue

After successfully completing my first merged contribution, I wanted to continue contributing to the USACO Guide repository.

This issue focuses on improving documentation for new USACO contestants by expanding the FAQ page with commonly asked questions that are currently missing.

---

## Understanding the Issue

### Problem Description

The current FAQ page does not answer several common questions covered by other USACO resources.

### Expected Behavior

The FAQ should contain additional questions and answers that help new users navigate contests, submissions, analyses, and test data.

### Current Behavior

Several common beginner questions are not covered.

### Affected Components

Potentially:

```text
content/1_General/USACO_FAQ.mdx
```

---

## Reproduction Process

### Environment Setup

Already completed during Contribution #1.

### Steps to Reproduce

1. Open the USACO FAQ page.
2. Compare it with the external FAQ resources linked in issue #3384.
3. Identify missing questions.

### Reproduction Evidence

Issue:
https://github.com/cpinitiative/usaco-guide/issues/3384

Comment:
https://github.com/cpinitiative/usaco-guide/issues/3384

Current findings:

Potential additions:

* How to submit solutions
* Where to find contest analyses
* Where to access test data
* Common beginner questions

---

## Solution Approach

### Analysis

The issue is intentionally open-ended. The best approach is to propose a small number of useful FAQ additions before making larger changes.

### Proposed Solution

Add 3–5 new FAQ entries that address frequently asked beginner questions.

### Implementation Plan

**Understand**

The FAQ is missing information commonly asked by new contestants.

**Match**

Existing FAQ entries provide the required structure and formatting.

**Plan**

1. Review current FAQ page.
2. Review linked FAQ resources.
3. Identify missing questions.
4. Draft answers.
5. Update FAQ page.
6. Test formatting.
7. Open PR.

**Implement**

Waiting for maintainer response.

**Evaluate**

Verify new questions render correctly and provide useful information.

---

## Testing Strategy

### Manual Testing

* [ ] Review FAQ page
* [ ] Verify formatting
* [ ] Verify links
* [ ] Verify answers are accurate

---

## Implementation Notes

### Current Progress

* Claimed issue #3384
* Commented on issue
* Requested maintainer guidance
* Began researching FAQ additions

### Current Status

Waiting for maintainer feedback before implementation.

### Branch

TBD

---

## Pull Request

PR Link:
TBD

Status:
Not Opened

---

## Learnings & Reflections

### Goals

* Improve documentation quality
* Learn documentation contribution workflow
* Complete a second contribution cycle

---

## Resources Used

* https://github.com/cpinitiative/usaco-guide/issues/3384
* https://blog.ktbyte.com/usaco-faq/
* https://alphastar.academy/usaco-info-and-preparation/
* https://ascendelearning.com/usaco-faq/
* https://www.stemivy.com/faq.html
