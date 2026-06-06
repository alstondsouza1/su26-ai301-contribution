# Contribution 1: Remove Ideone and repl.it from Running Code Online Recommendations

**Contribution Number:** 1
**Student:** Alston Dsouza
**Issue:** https://github.com/cpinitiative/usaco-guide/issues/5159
**Status:** Phase IV Complete

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

I cloned my fork of the USACO Guide repository and installed dependencies using Yarn.

```bash
git clone https://github.com/alstondsouza1/usaco-guide.git
cd usaco-guide
yarn install
yarn dev
```

The site ran successfully at:

```text
http://localhost:3000
```

### Steps to Reproduce

1. Run the USACO Guide project locally.
2. Navigate to `/general/running-code-online`.
3. Review the recommended online coding platforms.
4. Observe that Ideone and repl.it are listed.
5. Compare this behavior with issue #5159 requirements.

### Reproduction Evidence

* **Commit showing reproduction:** https://github.com/alstondsouza1/usaco-guide/commit/e0a076a0d
* **Screenshots/logs:** Verified locally through browser testing.
* **My findings:** Ideone and repl.it were still listed even though maintainers indicated they should be removed.

---

## Solution Approach

### Analysis

The issue was content-related rather than a software bug. The recommendations were stored directly in the MDX file used to generate the Running Code Online page.

### Proposed Solution

Remove the Ideone and repl.it recommendations and update the warning text to be platform-agnostic.

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** The page should only recommend contest-appropriate platforms.

**Match:** Similar recommendation content was already stored in the same MDX file.

**Plan:**

1. Remove the Ideone section.
2. Remove the repl.it section.
3. Update the contest privacy warning.
4. Verify the page renders correctly.
5. Open a pull request.

**Implement:**
Branch: https://github.com/alstondsouza1/usaco-guide/tree/update-running-code-online-recommendations

PR: https://github.com/cpinitiative/usaco-guide/pull/6238

**Review:**
Verified only the intended file was modified and followed repository contribution guidelines.

**Evaluate:**
Confirmed Ideone and repl.it no longer appear on the page and that the documentation renders correctly.

---

## Testing Strategy

### Unit Tests

* [x] Verify documentation builds successfully.
* [x] Verify modified MDX file renders correctly.
* [x] Verify warning text displays correctly.

### Integration Tests

* [x] Load Running Code Online page locally.
* [x] Confirm removed platforms no longer appear.

### Manual Testing

Verified locally that:

* Ideone no longer appears.
* repl.it no longer appears.
* Updated warning text appears correctly.
* Page renders successfully.

---

## Implementation Notes

### Week 1 Progress

* Selected issue #3573.
* Set up contribution repository.
* Forked USACO Guide.
* Investigated the issue.

### Week 2 Progress

* Determined issue #3573 was already resolved.
* Maintainer confirmed the issue was complete and closed it.
* Selected issue #5159.
* Set up local environment.
* Investigated affected file.
* Implemented requested changes.
* Opened pull request.

### Week 3 Progress

* Passed automated checks.
* Received maintainer review.
* Pull request approved.
* Pull request merged.

### Code Changes

* **Files modified:** content/1_General/Running_Code_Online.mdx
* **Key commits:** e0a076a0d
* **Approach decisions:** Kept the change focused to a single documentation file.

---

## Pull Request

**PR Link:** https://github.com/cpinitiative/usaco-guide/pull/6238

**PR Description:**

Removed Ideone and repl.it from the Running Code Online recommendations and updated the contest privacy warning.

**Maintainer Feedback:**

* Approved by @bqi343
* Pull request merged successfully

**Status:** Merged

---

## Learnings & Reflections

### Technical Skills Gained

* Open-source contribution workflow
* Git branching and pull requests
* Repository navigation
* MDX content editing
* Maintainer communication

### Challenges Overcome

My original issue (#3573) had already been implemented even though it remained open. I investigated the codebase, communicated with the maintainer, and successfully pivoted to another active issue.

### What I'd Do Differently Next Time

I would verify earlier whether an issue has already been implemented before investing significant time investigating it.

---

## Resources Used

* https://github.com/cpinitiative/usaco-guide/issues/3573
* https://github.com/cpinitiative/usaco-guide/issues/5159
* https://github.com/cpinitiative/usaco-guide/pull/6238
* https://github.com/cpinitiative/usaco-guide
* USACO Guide source code
* CodePath AI301 instructions
* Claude Code
