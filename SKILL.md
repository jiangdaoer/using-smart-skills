---
name: using-smart-skills
description: Interview users to clarify open-ended requirements, resolve unclear preferences or dissatisfaction, and choose suitable skills. Reuse decisions on follow-ups; fully specified tasks can proceed directly.
---

# Smart Skills

A self-contained workflow for understanding the user's intent, resolving decisions through an interview, and selecting the skills needed to deliver. All interview and routing rules are defined here; no other entry, interview, or routing skill is required. Specialist skills are optional execution capabilities selected for the task.

## 1. Establish what needs deciding

Check the available skill catalog, request, prior decisions, and accessible materials. On first use, briefly announce using-smart-skills and its purpose. Honor host entry rules and explicit skill choices. When a pending question concerns method suitability, feasibility, required inputs, or acceptance criteria, consult relevant specialist instructions or accessible evidence before framing the question or confirming the brief. Load only guidance needed for that decision, and bring any new constraints into the same interview. This informs clarification; it does not authorize implementation or start a second interview.

Start an interview when the intended result is not yet clear: an open-ended goal, an ambiguous preference, dissatisfaction whose cause is unresolved, or a consequential choice. Judge meaning in context, across domains and on follow-ups. Naming a deliverable or asking for an improvement does not establish the desired experience or success criteria. Explore relevant gaps even when a plausible default would let you produce something.

A fully specified request can proceed under existing authorization. Reuse prior answers; default only low-impact implementation details. When a request changes, reopen the affected decisions rather than the whole brief. Distinguish accessible facts to investigate from preferences and decisions the user must supply or delegate.

## 2. Interview through the decision tree

The goal is an explicit shared understanding, not merely enough information to start. Apply the interview to recommendations and planning as well as implementation.

Track the decisions shaping the result and their dependencies. Keep their status distinct: answered, explicitly delegated, unanswered, or waiting on evidence. A decision belongs in the tree when plausible answers would change the user-visible result, an important constraint, a success criterion, or the validity of the chosen method. Remove branches that do not meet that test; do not expand the tree merely because more details are imaginable. Scope comes from the request and the user's decisions. Keep the tree compactly in context, showing a brief unresolved-decisions summary when useful.

Work in rounds:

1. Identify open decisions whose prerequisites are settled. Prioritize those that could change the overall direction, rule out unsuitable approaches, or unlock other decisions; ask detail questions afterward. Group independent questions into a coherent round and split large sets into manageable batches while retaining the rest. Questions depending on an unanswered decision belong to a later round.
2. Number the questions in plain language and explain why the answer matters. When preferences are unformed, first ask about the user's purpose, experience, or dissatisfaction before proposing a preferred solution. If examples are needed, offer balanced contrasts and permit free-text alternatives. Recommend once grounded in the user's answers or applicable evidence; if the user directly requests a recommendation, give a provisional one with its assumptions and unresolved choice. Choose concrete discovery questions over a fixed questionnaire.
3. Receive the user's answers under section 3, then update the tree. For an answer that changes direction or unlocks a major branch, briefly restate your understanding in one sentence before the next question. If competing interpretations would change the result, clarify that ambiguity before pursuing the branch. Clear answers need no separate approval; ordinary details need no repeated paraphrase. An abstract preference or high-level option remains open where its meaning, consequences, or success criteria would change the result.
4. Probe a relevant trade-off, counterexample, or failure case when it exposes an assumption. Clarify contradictions and interpretations that affect the outcome. Reuse settled answers instead of challenging them to prolong the interview.

Investigate accessible facts yourself, or delegate investigation only when authorized. Keep evidence-dependent decisions open while working on independent questions. An absence of currently answerable questions does not resolve branches waiting on evidence.

When the user is unsure, use concrete contrasts or a small reversible sample to make the choice answerable, following the recommendation rule in step 2. Keep these aids provisional. A finished plan followed by "Does this work?" does not replace discovering the requirements that shape it. "I don't know" requests help; "use your judgment" delegates choices within its stated scope, not evidence or authorization.

Read [exploration.md](references/exploration.md) when intent is hard to express, dissatisfaction needs unpacking, or a plan's assumptions need examination. That reference supplies techniques; the interview, waiting, and completion rules remain here.

## 3. Ask and wait for an actual answer

For a decision needed to resolve requirements, ask in plain text in the final response and yield for the user's next message. Include only the context and provisional comparisons needed to answer. This pauses for input; it does not complete the task. Continue independent investigation when useful, but hold conclusions and work that depend on the answer.

Keep unresolved decisions pending without an answer deadline. Elapsed time, silence, a preselected option, tool acknowledgement such as accepted: true, a timeout, or a closed dialog is not an answer. If a required question dialog closes, carry the question into plain text and yield rather than reopening it repeatedly or assuming a choice. This skill cannot control the application's dialog lifetime.

Use asynchronous question tools only for genuinely optional input, subject to host rules. Keep necessary decisions necessary. Apply the host's fallback rules to optional unanswered input and identify assumptions as assumptions. Resume the tree from actual answers and reuse prior explicit delegation.

## 4. Confirm the completed understanding

End the interview only when all relevant branches are resolved: answers are concrete enough to guide the result, delegated decisions have explicit proposed resolutions, necessary evidence is available, and contradictions are settled. Exclusions or deferrals must be explicit and leave no unresolved dependency for the agreed work.

After a substantive interview, summarize the goal, scope, constraints, substantive choices, and success criteria. Ask the user to confirm that this captures the intended result, and wait before final recommendations or dependent implementation. For one narrow clarification, a clear answer that fully resolves the only open decision may itself confirm the updated understanding; do not add a separate confirmation turn. An explicit user summary or agreement already covering the same current brief also counts. Corrections reopen affected branches and require confirmation of the revised understanding. This confirms understanding developed through the interview, not an invented plan.

If the user ends or limits the interview, respect that instruction, state unresolved limits, and proceed only within their authorization; do not call the interview complete. Confirmation of an exploration-only brief does not itself request implementation. A fully specified task needing no interview does not acquire a new confirmation gate.

## 5. Select skills and deliver against the brief

Use the current catalog to match skills to the confirmed outcome, format, platform, and constraints. Candidate discovery and informed comparison can occur during the interview; a skill choice affecting the result is another decision in that tree.

- When several skills have similar descriptions or plausibly fit, make a shortlist of all genuinely relevant, distinct candidates. Read the candidate instructions needed to distinguish them; do not rank by name or description alone when their differences are unclear. List each candidate and explain its specific advantage, fit, and material limitation for this task. Separate competing approaches from complementary capabilities; collapse duplicate aliases.
- Recommend either one skill or a compatible combination, explain the division of work and why it best serves this brief, then invite the user to choose one, several, or another available option. Wait for the selection before dependent execution unless the user has already chosen or explicitly delegated the choice. Carry the selected choice forward without re-running the comparison.
- When only one skill clearly fits, explain briefly and use it. Load current-step instructions and dependencies only.
- When no skill adds value, work directly. If a requested capability is unavailable, disclose the gap and establish a feasible alternative without claiming it was used.

Carry the confirmed brief into each selected specialist: reuse the user's answers, constraints, and delegated choices before applying its workflow. Ask only about a genuinely new unresolved decision required by that specialist; do not ask the same question again in different words. If its requirements conflict with the brief, identify the concrete conflict and resolve only that part through the existing interview. Preserve explicit specialist approval requirements and user-selected workflows. Specialist use does not expand authorization.

Carry the confirmed brief into authorized work and verify against its success criteria. Maintain a compact record of decisions, assumptions, and blockers in context. When a long task or handoff risks losing material decisions, save a concise brief in the authorized workspace and refer to it on continuation; otherwise keep the record in the conversation. Do not claim a future preference or memory was saved unless the user explicitly requested it through a supported mechanism. Preserve the main objective through side questions and corrections. State actual completion, evidence, and limitations. Persist future preferences only on explicit request through a supported mechanism.
