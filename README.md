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

* `content/1_General/Running_Code_Online.mdx`
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

Merged

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

Merged

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

---

# Contribution 3: Improving Documentation Structure

**Contribution Number:** 3
**Student:** Alston Dsouza
**Issue:** https://github.com/apache/hamilton/issues/1043
**Status:** Phase IV In Progress

---

## Why I Chose This Issue

After completing two merged contributions to the USACO Guide repository, I wanted to contribute to a larger open-source project and continue improving my documentation contribution skills.

I chose this issue because it focuses on documentation structure and navigation. It matches my recent experience working with documentation pages, Markdown/MDX-style files, Git branches, pull requests, and maintainer feedback. I also wanted to learn how a larger Apache project organizes documentation, API reference pages, and contributor-facing resources.

---

## Understanding the Issue

### Problem Description

As Apache Hamilton has grown, parts of its documentation have become harder to navigate because different types of content are grouped together.

Issue #1043 identifies several documentation-structure improvements:

1. The Integrations section mixes plugin guides with application examples.
2. The API reference does not have a dedicated plugin section.
3. The Lifecycle Adapters section mixes lifecycle API interfaces with concrete adapter implementations.

### Expected Behavior

The documentation should clearly separate different types of content so users can more easily find what they need.

Plugin guides, cookbook examples, lifecycle API interfaces, and concrete adapter implementations should be organized into clearer sections.

### Current Behavior

Before my changes:

* `docs/integrations/` contained both plugin guides and application examples.
* FastAPI and Streamlit appeared alongside dlt, Ibis, and dbt.
* `docs/reference/lifecycle-hooks/` contained both lifecycle interfaces and concrete adapter implementations.
* The API reference did not contain a separate plugin reference section.

### Affected Components

```text
docs/index.md
docs/integrations/
docs/reference/lifecycle-hooks/
docs/ecosystem/index.md
docs/code-comparisons/
examples/
```

---

## Reproduction Process

### Environment Setup

I forked the Apache Hamilton repository and cloned my fork locally.

```bash
git clone https://github.com/alstondsouza1/hamilton.git
cd hamilton
git remote add upstream https://github.com/apache/hamilton.git
git fetch upstream
git switch -c docs-1043-structure
```

I reviewed the documentation setup instructions and attempted to install the documentation dependencies.

```bash
python -m pip install --group docs
```

One challenge was that my local Python version was Python 3.9.6, while Apache Hamilton requires Python 3.10.1 or newer. I also attempted to use a Python 3.11 Docker container, but Docker was not running locally.

### Steps to Reproduce

1. Open `docs/index.md`.
2. Review the main documentation navigation.
3. Open `docs/integrations/index.rst`.
4. Observe that plugin guides and application examples are grouped together.
5. Open `docs/reference/lifecycle-hooks/index.rst`.
6. Observe that lifecycle API interfaces and concrete adapter implementations are listed together.
7. Search the repository for links pointing to the affected documentation paths.

### Reproduction Evidence

* **Commit showing reproduction:** https://github.com/alstondsouza1/hamilton/tree/docs-1043-structure
* **Screenshots/logs:** Not applicable; this is a documentation-structure issue.
* **My findings:** The documentation structure matched the issue description. Plugin guides, cookbook-style examples, lifecycle APIs, and adapter implementations were not clearly separated.

---

## Solution Approach

### Analysis

This was a documentation-structure issue rather than a code bug. The root problem was that documentation sections had grown over time and different types of content were grouped together.

The main risk was that moving documentation files could break navigation, toctree entries, ecosystem links, comparison pages, or example README links. Because of this, I needed to update both the documentation structure and any references to the old paths.

### Proposed Solution

I reorganized the documentation into clearer sections:

```text
docs/plugins/
docs/cookbook/
docs/reference/lifecycle-hooks/
docs/reference/plugins/
```

The goal was to separate:

* Plugin guides from cookbook examples.
* Lifecycle API interfaces from concrete plugin/adapter implementations.
* User-facing guides from API reference pages.

### Implementation Plan

Using UMPIRE framework:

**Understand:**
The documentation needs clearer structure because plugin guides, cookbook examples, lifecycle APIs, and concrete adapter implementations are currently grouped together.

**Match:**
The repository already uses Sphinx, reStructuredText, Markdown, and toctree navigation. Similar documentation sections already use index files and structured navigation entries.

**Plan:**

1. Create a feature branch.
2. Split the Integrations section into Plugins and Cookbook.
3. Move dlt, Ibis, and dbt documentation into `docs/plugins/`.
4. Move FastAPI and Streamlit documentation into `docs/cookbook/`.
5. Update `docs/index.md` navigation.
6. Rename Lifecycle Adapters to Lifecycle API.
7. Keep lifecycle interfaces in `docs/reference/lifecycle-hooks/`.
8. Create `docs/reference/plugins/` for concrete adapter/plugin implementations.
9. Update internal documentation links.
10. Update affected example README links.
11. Check for stale paths and missing documentation targets.
12. Push the branch and open a pull request.

**Implement:**
Branch: https://github.com/alstondsouza1/hamilton/tree/docs-1043-structure
Pull Request: https://github.com/apache/hamilton/pull/1647

**Review:**
I checked the changes for broken paths, stale references, conflict markers, whitespace issues, and unintended unrelated changes. I also organized the work into focused commits.

**Evaluate:**
The pull request is open and awaiting CI and maintainer review. I could not complete the full documentation build locally due to Python version and Docker limitations, but I documented this limitation and expect CI to run the full build.

---

## Testing Strategy

### Unit Tests

* [x] Verify documentation files were moved into the intended sections.
* [x] Verify moved documentation pages still exist at their new paths.
* [x] Verify Sphinx toctree targets exist.

### Integration Tests

* [x] Verify documentation navigation was updated.
* [x] Verify internal documentation links were updated.
* [x] Verify affected example README links were updated.

### Manual Testing

I completed the following manual checks:

* Reviewed the documentation structure.
* Separated Plugins and Cookbook.
* Separated lifecycle interfaces and plugin adapters.
* Added Plugin API Reference.
* Updated documentation navigation.
* Updated internal links.
* Updated affected example links.
* Checked for stale paths.
* Verified documentation targets exist.
* Verified the Git worktree was clean before pushing.
* Pushed the feature branch to my fork.
* Opened the pull request.

The full documentation build is pending CI because my local environment did not meet the required Python version.

---

## Implementation Notes

### Week 5 Progress

I selected Apache Hamilton issue #1043, reviewed the issue requirements, commented on the issue expressing interest, and added the contribution to my README.

I also reviewed the existing documentation structure and chose a focused approach: splitting documentation into clearer Plugins, Cookbook, Lifecycle API, and Plugin API Reference sections.

### Week 6 Progress

I implemented the documentation restructuring, updated navigation and links, pushed my feature branch, and opened pull request #1647.

I also corrected my Git setup after initially working in a checkout where the Apache repository was configured as `origin`. I created my personal fork, configured `origin` and `upstream` correctly, preserved my feature branch, restored `main`, and pushed only my feature branch to my fork.

### Code Changes

* **Files modified:** Documentation files under `docs/`, `docs/integrations/`, `docs/plugins/`, `docs/cookbook/`, `docs/reference/lifecycle-hooks/`, `docs/reference/plugins/`, and affected example README files.
* **Key commits:**

  * `797c2c77` — split integrations into plugins and cookbook
  * `5402ef19` — separate lifecycle api from plugin adapters
  * `e5d80e64` — fix example links after moving the docs
* **Approach decisions:** I chose to keep the work documentation-focused and split it into several commits so maintainers can review each part more easily.

---

## Pull Request

**PR Link:** https://github.com/apache/hamilton/pull/1647

**PR Description:**
This PR improves the Apache Hamilton documentation structure by separating plugin guides, cookbook examples, lifecycle APIs, and plugin API reference documentation into clearer sections. It also updates documentation navigation and affected internal links.

**Maintainer Feedback:**

* Pending: Waiting for CI and maintainer review.

**Status:** Awaiting review

---

## Learnings & Reflections

### Technical Skills Gained

I gained experience working with Sphinx documentation, reStructuredText, Markdown, documentation navigation, API reference organization, Git remotes, forks, feature branches, and pull requests across repositories.

### Challenges Overcome

The main challenge was that moving documentation files required more than simply changing file locations. Navigation files, ecosystem pages, comparison pages, and example README files also referenced the old paths, so I had to search the repository and update related links.

I also corrected my Git remote setup before opening the pull request so that my changes were pushed from my personal fork instead of the upstream Apache repository.

### What I'd Do Differently Next Time

Next time, I would fork and clone my personal fork before making any changes. I would also confirm the required Python version and documentation build dependencies before starting implementation so I can run the full documentation build earlier.

---

## Resources Used

* https://github.com/apache/hamilton/issues/1043
* https://github.com/apache/hamilton/pull/1647
* https://github.com/apache/hamilton/pull/1199
* https://github.com/apache/hamilton
* https://github.com/alstondsouza1/hamilton
* https://github.com/alstondsouza1/hamilton/tree/docs-1043-structure
* `docs/README.md`
* CodePath AI301 materials
