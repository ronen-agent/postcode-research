# GitHub Workflow for Automated Proposals

This workflow applies when the cloud agent is authorized to prepare and publish proposals for <https://github.com/ronen/postcode-research>. It does not govern interactive local editing or authorize an otherwise unrequested task. The task's procedure defines what to investigate and change; the schedule prompt defines timing, execution environment, model, and notifications.

## 1. Identity and access

Use the GitHub connection authenticated as `ronen-agent`. The upstream repository is `ronen/postcode-research`; proposed changes belong on branches in the agent account's fork, with draft pull requests targeting upstream.

Verify the connected identity and the ability to read upstream, write to the fork, and open cross-repository PRs. Do not substitute the human's credentials or request upstream write access to overcome a limitation. If an operation is unavailable, report the specific limitation and preserve useful partial work without claiming publication succeeded.

## 2. Obtain the current inputs and proposal history

At the start of each run, read upstream's current root [AGENTS.md](../AGENTS.md), this workflow, and the applicable task procedure from its default branch. Do this explicitly even if the environment loads repository instructions automatically. Use the actual default branch name (currently `main`), record the revision used, and obtain the task's inputs from that revision. Do not rely solely on an environment's initial checkout, a stale fork, or remembered document copies.

Inspect relevant open, merged, and closed upstream PRs, including proposals from the agent's fork. Read their reports and review decisions where relevant: they may contain pending findings or rejection reasons absent from the default branch.

## 3. Prepare the fork and proposal branch

When there are changes worth proposing, locate `ronen-agent`'s existing fork of upstream and verify its upstream relationship rather than trusting its name. If no fork exists, create one under `ronen-agent`; normally it will be named `ronen-agent/postcode-research`. Reuse this fork across runs. Do not overwrite an unrelated repository occupying that name. If the available tools cannot create or access the fork, report that setup requirement instead of changing the publication model.

Resolve the latest upstream default-branch revision and create each new proposal branch in the fork directly from that revision. If the available tools cannot establish that revision in the fork, report the limitation.

Synchronizing the fork's default branch is optional housekeeping and must not be a prerequisite for preparing a proposal. If synchronizing it, verify that the update is a fast-forward and use a non-forced update guarded by the fork branch's expected current revision. Preserve divergent or fork-only work; do not reset or force-push the branch.

Use a descriptive, unique branch name, such as `<task-name>/YYYY-MM-DD`, adding a distinguishing suffix if needed. Keep existing proposal branches separate.

If an existing open PR already covers the proposed change, avoid opening a duplicate. Update an existing automation-owned branch only when it contains no intervening human changes and the update remains within its scope; otherwise report the overlap for review.

## 4. Publish a draft PR

Before publication, recheck upstream and relevant open PRs for intervening changes and duplicate proposals. If upstream has changed, reconcile and revalidate the proposal against the new revision before publishing.

Complete the task procedure's content checks and inspect the final diff, document consistency, and relative links. Commit only the intended files, push the proposal branch to the agent's fork, and open a draft PR with that fork branch as the head and the upstream default branch as the base.

Explain the proposed changes, their rationale, validation, limitations, and decisions needed. Include the task's report and primary-source links where applicable. Check public artifacts for private chat context and credentials before publishing. Return the PR URL and a concise outcome for the invoking task to report.

When there are no changes worth proposing, create no fork, proposal branch, commit, or PR. If publication fails, retain prepared work where possible and report the failure without claiming a PR exists.

## 5. Human integration

The human reviews and merges or rejects proposals. Automated runs must never write to upstream branches, merge PRs, enable auto-merge, bypass protections, force-push, delete branches or the fork, or modify repository settings. Fast-forwarding the fork's default branch from upstream is permitted as described above.
