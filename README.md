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

### What I'd Do Differently Next Time

I would verify earlier whether an issue had already been implemented before investing significant time investigating it.

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
**Status:** Phase IV Complete (Merged)

---

## Why I Chose This Issue

After successfully completing my first merged contribution, I wanted to continue contributing to the USACO Guide repository.

This issue focused on improving documentation for new USACO contestants by expanding the FAQ page with commonly asked questions that were not currently covered.

I also wanted additional experience working through the full open-source contribution cycle, including receiving maintainer feedback, revising my work, and getting a pull request merged.

---

## Understanding the Issue

### Problem Description

The USACO FAQ page did not answer several common questions that appeared in other USACO-related FAQ resources.

Issue #3384 specifically mentioned expanding the FAQ to address questions commonly asked by new contestants.

### Expected Behavior

The FAQ should include useful information that helps users understand USACO processes and navigate contest-related information.

### Current Behavior

Some commonly asked beginner questions were not answered on the existing FAQ page.

### Affected Components

```text
content/1_General/USACO_FAQs.mdx
```

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

1. Open the USACO FAQ page.
2. Review the questions currently listed.
3. Compare the page with external FAQ resources referenced in issue #3384.
4. Identify common questions not currently addressed.

### Reproduction Evidence

Issue:

https://github.com/cpinitiative/usaco-guide/issues/3384

The issue discussion identified opportunities to expand the FAQ with additional beginner-focused information.

---

## Solution Approach

### Analysis

The issue was intentionally open-ended and required contributors to identify useful FAQ additions while avoiding duplication of existing content.

### Proposed Solution

Add a new FAQ entry explaining where users can view their contest history, scores, current division, and promotion information.

### Implementation Plan

1. Review the current FAQ page.
2. Review linked FAQ resources.
3. Identify missing beginner questions.
4. Draft a new FAQ entry.
5. Verify formatting and rendering.
6. Submit a pull request.
7. Address maintainer feedback.

### Implement

Branch:

```text
expand-usaco-faq
```

PR:

https://github.com/cpinitiative/usaco-guide/pull/6246

### Evaluate

Verified the new FAQ entry rendered correctly and integrated with the existing FAQ structure.

Maintainer feedback was addressed through multiple revisions before merge.

---

## Testing Strategy

### Manual Testing

* Verified FAQ page builds successfully.
* Verified new FAQ entry appears correctly.
* Verified formatting renders correctly.
* Ran formatting checks on the modified MDX file.
* Confirmed no unrelated files were modified.

---

## Implementation Notes

### Week 3 Progress

* Claimed issue #3384.
* Reviewed existing FAQ content.
* Researched related FAQ resources.
* Drafted additional FAQ content.
* Opened pull request.

### Week 4 Progress

* Received community feedback regarding rankings visibility.
* Updated FAQ wording.
* Received maintainer review.
* Removed duplicate FAQ entries that overlapped with existing content.
* Refined wording based on maintainer suggestions.
* Pull request approved and merged.

### Code Changes

Files Modified:

```text
content/1_General/USACO_FAQs.mdx
```

Commits:

```text
4cb1ef5
0088503
374703e
0205f96
```

---

## Pull Request

PR:

https://github.com/cpinitiative/usaco-guide/pull/6246

Status:

Merged ✅

Maintainer Feedback:

* Community feedback suggested clarifying rankings availability.
* Maintainer identified duplicate FAQ entries.
* Duplicate questions were removed.
* Wording was refined based on maintainer suggestions.
* Final version approved and merged by @bqi343.

---

## Learnings & Reflections

### Technical Skills Gained

* Documentation contributions using MDX
* Git branching and pull request workflow
* Responding to code review feedback
* Iterating on contributions based on maintainer suggestions
* Open-source collaboration

### Challenges Overcome

My initial proposal included multiple FAQ additions. During review, the maintainer pointed out that some questions duplicated information already available elsewhere in the FAQ.

I revised the contribution, removed duplicate content, refined the wording, and successfully worked through the review process until the pull request was approved and merged.

### What I'd Do Differently Next Time

I would spend more time reviewing existing documentation before proposing additions to reduce the likelihood of overlapping content.

---

## Resources Used

* Issue #3384
* PR #6246
* USACO Guide source code
* https://blog.ktbyte.com/usaco-faq/
* https://alphastar.academy/usaco-info-and-preparation/
* https://ascendelearning.com/usaco-faq/
* https://www.stemivy.com/faq.html
* CodePath AI301 materials
