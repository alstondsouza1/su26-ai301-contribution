# Contribution 1: show a message if firebase fails to connect

**Contribution Number:** 1
**Student:** Alston Dsouza
**Issue:** https://github.com/cpinitiative/usaco-guide/issues/3573
**Status:** Phase II Complete

---

## Why I Chose This Issue

I chose issue #3573, "show a message if firebase fails to connect," because it matches my experience with JavaScript, React, Next.js, and frontend development. The USACO Guide project uses React, Next.js, TypeScript, Tailwind CSS, and Firebase, which are technologies closely related to the web development projects I have worked on.

This issue is labeled as a good first issue and appears to have a clear and manageable scope for my first open source contribution. From reading the issue discussion, I understand that some users may experience Firebase connection issues and may need clearer guidance about enabling long polling. I hope to learn more about how a large open source project handles user-facing messages, settings pages, and Firebase-related functionality.

---

## Understanding the Issue

### Problem Description

Some users may experience Firebase connection issues while using the USACO Guide website. The issue suggests adding a clearer message to help users understand that enabling long polling may help resolve certain Firebase connection problems.

### Expected Behavior

Users should receive clear guidance when Firebase connection issues occur and understand when the long polling setting may help solve the problem.

### Current Behavior

The issue discussion suggested that users needed a clearer message regarding Firebase connection issues and the long polling setting. However, after investigating the current codebase, I found that a message already exists on the settings page.

### Affected Components

* Settings page
* Long polling option
* Firebase-related functionality
* `src/components/Settings/General.tsx`

---

## Reproduction Process

### Environment Setup

I cloned my fork of the USACO Guide repository and installed the project dependencies using Yarn.

Commands used:

```bash
git clone https://github.com/alstondsouza1/usaco-guide.git
cd usaco-guide
yarn install
yarn dev
```

The setup completed successfully. Yarn displayed some peer dependency warnings, but the development server launched correctly and the website was accessible locally.

### Steps to Reproduce

1. Clone the USACO Guide repository.
2. Run `yarn install`.
3. Start the application using `yarn dev`.
4. Open `http://localhost:3000`.
5. Navigate to the Settings page.
6. Locate the "Use Long Polling" option.
7. Review the message displayed next to the setting.

### Reproduction Evidence

* **Working Branch:** https://github.com/alstondsouza1/usaco-guide/tree/investigate-firebase-long-polling-message
* **Relevant File:** `src/components/Settings/General.tsx`
* **Screenshots/logs:** Local development server running successfully.
* **My Findings:** The settings page already contains the message:

> "Enable this option ONLY if you encounter issues connecting to Firebase (nothing loads)."

This appears to match the maintainer's requested wording from the issue discussion.

---

## Solution Approach

### Analysis

After setting up the project locally and reviewing the settings page implementation, I found that the requested message already exists within the current codebase. The message is rendered in `src/components/Settings/General.tsx` alongside the "Use Long Polling" setting.

Because the GitHub issue remains open despite the message being present, it is unclear whether the issue is already resolved or whether maintainers expect additional functionality.

### Proposed Solution

Before making any code changes, I contacted the maintainers through the GitHub issue to clarify whether:

1. The issue should be considered resolved.
2. Additional functionality is expected.
3. A dynamic Firebase connection failure message should be implemented instead of the existing static message.

### Implementation Plan

Using UMPIRE framework:

**Understand:**
The issue requests a message to help users experiencing Firebase connection problems.

**Match:**
The existing implementation already contains a message attached to the long polling setting.

**Plan:**

1. Wait for maintainer clarification on issue #3573.
2. Determine whether the existing implementation satisfies the issue requirements.
3. If additional work is required, identify where Firebase connection failures are handled.
4. Design and implement any requested improvements.
5. Test changes locally before opening a pull request.

**Implement:**
Not started yet. Awaiting maintainer feedback.

**Review:**
Follow the project's contribution guidelines and coding standards before making any changes.

**Evaluate:**
Verify that users receive appropriate guidance when Firebase connection issues occur and confirm any requested behavior works as expected.

---

## Testing Strategy

### Unit Tests

* [ ] Verify settings page renders correctly.
* [ ] Verify long polling setting is displayed.
* [ ] Verify Firebase guidance message is displayed.

### Integration Tests

* [ ] Verify settings page loads successfully.
* [ ] Verify long polling option can be toggled.

### Manual Testing

Successfully verified the message appears on the settings page while running the project locally.

---

## Implementation Notes

### Week 1 Progress

Completed Phase I setup activities. Created the Contribution README repository, selected issue #3573, reviewed the issue discussion, and chose the issue because it aligns with my web development experience and learning goals.

### Week 2 Progress

Successfully:

* Forked the USACO Guide repository.
* Installed dependencies using Yarn.
* Ran the project locally.
* Located the relevant settings page component.
* Investigated the existing implementation.
* Confirmed the requested Firebase guidance message already exists.
* Posted a follow-up question on the GitHub issue requesting clarification from maintainers.

### Code Changes

**Files modified:** None yet

**Key Branch:**

* investigate-firebase-long-polling-message

**Approach Decisions:**

* Investigated the current implementation before making changes.
* Chose to request maintainer clarification before modifying working functionality.
* Documented findings thoroughly for future reference.

---

## Pull Request

**PR Link:** TBD

**PR Description:** TBD

**Maintainer Feedback:**

* Awaiting response regarding issue status and expected behavior.

**Status:** Awaiting maintainer clarification

---

## Learnings & Reflections

### Technical Skills Gained

* Improved familiarity with open source contribution workflows.
* Learned how to set up and run a large React/Next.js codebase locally.
* Practiced navigating unfamiliar codebases and tracing issue discussions to source code.

### Challenges Overcome

The biggest challenge was determining whether the issue still exists because the requested functionality appears to already be present in the codebase.

### What I'd Do Differently Next Time

I would verify whether the issue is already implemented earlier in the investigation process before assuming work remains to be completed.

---

## Resources Used

* https://github.com/cpinitiative/usaco-guide/issues/3573
* https://github.com/cpinitiative/usaco-guide
* USACO Guide README
* USACO Guide source code
* CodePath AI301 Phase I Instructions
* CodePath AI301 Phase II Instructions
* First Contributions Tutorial
