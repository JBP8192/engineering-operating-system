\# Review Request Template



\*\*Template ID:\*\* TPL-700-005

\*\*Title:\*\* Review Request Template

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Independent Auditor

\*\*Related Documents:\*\*



\* `200\_organization/COMMUNICATION\_MODEL.md`

\* `200\_organization/RACI\_MATRIX.md`

\* `100\_governance/AGENT\_TESTING\_PROCEDURE.md`

\* `700\_templates/WORK\_PACKAGE\_REQUEST\_TEMPLATE.md`



\---



\# 1. Purpose



This template defines the standard structure for requesting a review within the Engineering Operating System.



A Review Request is used when an artifact, decision, prompt, workflow, architecture, requirement, risk or agent output must be independently checked before it can be accepted, baselined or approved.



The purpose is to ensure that reviews are traceable, scoped, evidence-based and independent.



\---



\# 2. Review Request Metadata



| Field                | Value                                          |

| -------------------- | ---------------------------------------------- |

| Review Request ID    | RR-YYYY-NNN                                    |

| Title                | TBD                                            |

| Created Date         | TBD                                            |

| Requested by         | TBD                                            |

| Reviewer             | TBD                                            |

| Supporting Reviewers | TBD                                            |

| Priority             | Low / Medium / High / Critical                 |

| Risk Class           | C0 / C1 / C2 / C3 / C4 / C5 / C6               |

| Status               | Open / In Progress / Review Complete / Blocked |

| Related Project      | TBD                                            |

| Related Work Package | TBD                                            |

| Related Artifact     | TBD                                            |



\---



\# 3. Review Objective



Describe what the review shall determine.



Examples:



\* determine whether the artifact is complete,

\* determine whether the decision is traceable,

\* determine whether the prompt follows governance rules,

\* determine whether the architecture is internally consistent,

\* determine whether safety or compliance assumptions are sufficiently documented.



```text

Review Objective:



TBD

```



\---



\# 4. Artifact Under Review



| Field               | Value                                                                              |

| ------------------- | ---------------------------------------------------------------------------------- |

| Artifact Name       | TBD                                                                                |

| Artifact Type       | Requirement / ADR / Prompt / Workflow / Architecture / Risk / Test / Documentation |

| Artifact Location   | TBD                                                                                |

| Artifact Version    | TBD                                                                                |

| Artifact Owner      | TBD                                                                                |

| Change Under Review | TBD                                                                                |



\---



\# 5. Review Scope



\## In Scope



List what the review shall explicitly check.



```text

In Scope:



\- TBD

```



\## Out of Scope



List what the review shall not check.



```text

Out of Scope:



\- TBD

```



\---



\# 6. Review Criteria



The reviewer shall check the artifact against the following criteria.



| Criterion                          |      Required | Result |

| ---------------------------------- | ------------: | ------ |

| Alignment with EOS Constitution    |           Yes | TBD    |

| Alignment with AI Organization     |           Yes | TBD    |

| Alignment with RACI Matrix         | If applicable | TBD    |

| Alignment with Communication Model | If applicable | TBD    |

| Completeness                       |           Yes | TBD    |

| Internal consistency               |           Yes | TBD    |

| Traceability                       |           Yes | TBD    |

| Risks identified                   |           Yes | TBD    |

| Assumptions documented             |           Yes | TBD    |

| Open questions documented          |           Yes | TBD    |

| Required evidence identified       | If applicable | TBD    |

| Human approval needed identified   | If applicable | TBD    |

| No agent self-approval             |           Yes | TBD    |



\---



\# 7. Evidence Provided



List the evidence available for review.



| Evidence                        | Location | Provided |

| ------------------------------- | -------- | -------- |

| Source artifact                 | TBD      | Yes / No |

| Related requirement             | TBD      | Yes / No |

| Related ADR                     | TBD      | Yes / No |

| Related risk                    | TBD      | Yes / No |

| Related test                    | TBD      | Yes / No |

| Related work package            | TBD      | Yes / No |

| Related prompt or specification | TBD      | Yes / No |



\---



\# 8. Review Questions



The reviewer shall answer:



1\. Is the artifact understandable?

2\. Is the artifact complete enough for its purpose?

3\. Are assumptions clearly marked?

4\. Are risks clearly identified?

5\. Are open questions clearly listed?

6\. Are decisions traceable?

7\. Is required evidence available or identified?

8\. Does the artifact remain within the authority of its owner?

9\. Does the artifact require Human Owner approval?

10\. Can the artifact be accepted, accepted with conditions or rejected?



\---



\# 9. Finding Classification



Findings shall be classified as:



| Severity       | Meaning                                                      |

| -------------- | ------------------------------------------------------------ |

| Blocker        | Artifact cannot be accepted. Critical rework required.       |

| Major          | Significant issue. Rework required before normal acceptance. |

| Minor          | Small issue. Acceptance may be possible with follow-up.      |

| Observation    | Not blocking, but relevant information.                      |

| Recommendation | Suggested improvement.                                       |



\---



\# 10. Review Findings



| ID    | Severity | Finding | Required Action | Owner | Status |

| ----- | -------- | ------- | --------------- | ----- | ------ |

| F-001 | TBD      | TBD     | TBD             | TBD   | Open   |



\---



\# 11. Review Result



The final review result shall be one of:



| Result                   | Meaning                                                |

| ------------------------ | ------------------------------------------------------ |

| Accepted                 | Artifact may be used as intended.                      |

| Accepted with Conditions | Artifact may be used only under listed conditions.     |

| Rejected                 | Artifact must be reworked before use.                  |

| Deferred                 | Review cannot be completed due to missing information. |



\---



\# 12. Conditions



If the result is `Accepted with Conditions`, list all conditions.



```text

Conditions:



\- TBD

```



\---



\# 13. Required Rework



List all required rework before acceptance.



```text

Required Rework:



\- TBD

```



\---



\# 14. Follow-up Actions



| Action ID | Action | Owner | Priority | Due Date | Status |

| --------- | ------ | ----- | -------- | -------- | ------ |

| RA-001    | TBD    | TBD   | TBD      | TBD      | Open   |



\---



\# 15. Documentation Impact



Define what must be updated after review.



| Documentation Item    | Required | Target Location                            |

| --------------------- | -------- | ------------------------------------------ |

| Backlog Update        | Yes / No | `100\_governance/EOS\_FOUNDATION\_BACKLOG.md` |

| ADR Update            | Yes / No | TBD                                        |

| Risk Update           | Yes / No | TBD                                        |

| Requirement Update    | Yes / No | TBD                                        |

| Agent Registry Update | Yes / No | TBD                                        |

| Changelog Entry       | Yes / No | `CHANGELOG.md`                             |

| Lessons Learned       | Yes / No | `900\_lessons\_learned/`                     |



\---



\# 16. Reviewer Statement



```text

Reviewer Statement:



I reviewed the artifact according to the defined scope and criteria.



Result:



TBD



Rationale:



TBD

```



\---



\# 17. Approval



| Role                    | Name | Decision                       | Date |

| ----------------------- | ---- | ------------------------------ | ---- |

| Reviewer                | TBD  | Accepted / Rejected / Deferred | TBD  |

| Human Owner if required | TBD  | Approved / Rejected / Deferred | TBD  |



\---



\# 18. Change History



| Version | Date | Change                          | Author   |

| ------- | ---- | ------------------------------- | -------- |

| 0.1     | TBD  | Initial Review Request template | EOS Team |



