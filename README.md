# Contribution 1: show a message if firebase fails to connect

**Contribution Number:** 1
**Student:** Alston Dsouza
**Issue:** https://github.com/cpinitiative/usaco-guide/issues/3573
**Status:** Phase II Complete

---

## Why I Chose This Issue

I chose issue #3573, "show a message if firebase fails to connect," because it matches my experience with JavaScript, React, Next.js, and frontend development. The USACO Guide project uses React, Next.js, TypeScript, Tailwind CSS, and Firebase, which are technologies closely related to the web development projects I have worked on.

This issue was labeled as a good first issue and appeared to have a clear and manageable scope for my first open source contribution.

---

## Understanding the Issue

### Problem Description

The issue requested a message to help users understand that enabling long polling may help resolve Firebase connection problems.

### Expected Behavior

Users experiencing Firebase connection issues should receive clear guidance about enabling long polling.

### Current Behavior

After investigating the current codebase, I found that the requested message already exists on the settings page.

### Affected Components

* Settings page
* Long polling option
* Firebase-related functionality
* `src/components/Settings/General.tsx`

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

The application started successfully and was accessible at `http://localhost:3000`.

### Steps to Reproduce

1. Clone the USACO Guide repository.
2. Run `yarn install`.
3. Run `yarn dev`.
4. Open `http://localhost:3000`.
5. Navigate to the Settings page.
6. Locate the "Use Long Polling" option.
7. Review the message displayed next to the setting.

### Reproduction Evidence

**Working Branch:**
https://github.com/alstondsouza1/usaco-guide/tree/investigate-firebase-long-polling-message

**Relevant File:**
`src/components/Settings/General.tsx`

**Finding:**

The settings page already contains the message:

> "Enable this option ONLY if you encounter issues connecting to Firebase (nothing loads)."

This matches the wording requested by the maintainers in the GitHub issue discussion.

---

## Solution Approach

### Analysis

After reviewing the issue discussion and examining the current implementation, I determined that the requested functionality had already been implemented in the codebase.

The message requested by the maintainers exists in:

```text
src/components/Settings/General.tsx
```

### Proposed Solution

No code changes were necessary.

Instead, I contacted the maintainers through the GitHub issue to confirm whether the issue was already resolved or if additional behavior was still expected.

### Maintainer Response

Maintainer **@bqi343** responded:

> "yes I think it's fine now"

The issue was subsequently closed by the maintainer as completed.

### Implementation Plan

1. Reproduce the issue locally.
2. Locate the relevant implementation.
3. Compare the implementation with the issue requirements.
4. Request maintainer clarification.
5. Document findings.
6. Move to a new issue for an actual code contribution.

---

## Testing Strategy

### Manual Testing

Successfully verified:

* Settings page loads correctly.
* Long polling option is displayed.
* Firebase guidance message is displayed.
* Message matches the wording requested in the issue discussion.

### Result

Issue requirements appear to already be satisfied in the current codebase.

---

## Implementation Notes

### Week 1 Progress

* Completed Phase I setup activities.
* Selected issue #3573.
* Created contribution repository.
* Reviewed issue discussion.

### Week 2 Progress

Successfully:

* Forked the USACO Guide repository.
* Installed dependencies using Yarn.
* Ran the project locally.
* Investigated the settings page implementation.
* Located the existing Firebase guidance message.
* Confirmed the message matched the requested wording.
* Contacted project maintainers for clarification.
* Received confirmation that the issue was already resolved.
* Observed the maintainer close the issue.

### Code Changes

**Files modified:** None

**Branch Created:**

* investigate-firebase-long-polling-message

### Outcome

No code contribution was required because the issue had already been implemented and verified by the maintainer.

---

## Pull Request

**PR Link:** N/A

**Status:** No pull request required.

**Reason:**

The issue was confirmed by the maintainer as already resolved and was closed after my investigation.

---

## Learnings & Reflections

### Technical Skills Gained

* Set up and ran a large Next.js and TypeScript project locally.
* Navigated an unfamiliar open source codebase.
* Traced issue discussions to source code implementations.
* Practiced communicating findings with maintainers.

### Challenges Overcome

The main challenge was determining whether the issue still existed because the requested functionality appeared to already be present.

### What I'd Do Differently Next Time

I would verify earlier whether an issue has already been implemented before assuming development work remains.

### Key Lesson

Before beginning implementation, always reproduce the issue and verify it still exists. Sometimes an issue remains open even though the requested functionality has already been added.

---

## Resources Used

* https://github.com/cpinitiative/usaco-guide/issues/3573
* https://github.com/cpinitiative/usaco-guide
* USACO Guide README
* USACO Guide source code
* CodePath AI301 Phase I Instructions
* CodePath AI301 Phase II Instructions
* First Contributions Tutorial
