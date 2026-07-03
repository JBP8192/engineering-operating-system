\# Work Package Request Template



\*\*Template ID:\*\* TPL-700-004

\*\*Title:\*\* Work Package Request Template

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering OS Orchestrator

\*\*Related Documents:\*\*



\* `200\_organization/COMMUNICATION\_MODEL.md`

\* `200\_organization/RACI\_MATRIX.md`

\* `100\_governance/AGENT\_TESTING\_PROCEDURE.md`



\---



\# 1. Purpose



This template defines the standard structure for assigning work packages within the Engineering Operating System.



A Work Package Request is used when the Engineering OS Orchestrator assigns a defined task to one or more agents.



The purpose is to make agent work traceable, scoped, reviewable and documentable.



\---



\# 2. Work Package Request



\## Work Package Metadata



| Field             | Value                                        |

| ----------------- | -------------------------------------------- |

| Work Package ID   | WP-YYYY-NNN                                  |

| Title             | TBD                                          |

| Created Date      | TBD                                          |

| Requested by      | Engineering OS Orchestrator                  |

| Assigned to       | TBD                                          |

| Supporting Agents | TBD                                          |

| Priority          | Low / Medium / High / Critical               |

| Risk Class        | C0 / C1 / C2 / C3 / C4 / C5 / C6             |

| Status            | Open / In Progress / Review / Done / Blocked |

| Related Project   | TBD                                          |

| Related Artifact  | TBD                                          |



\---



\# 3. Context



Describe the background of the task.



Include:



\* why this work package exists,

\* which previous decision or request triggered it,

\* which project or EOS capability it supports,

\* relevant links to documents, issues or previous work.



```text

Context:



TBD

```



\---



\# 4. Objective



Describe the expected result of the work package.



The objective should be specific enough that the assigned agent can determine whether the task is complete.



```text

Objective:



TBD

```



\---



\# 5. Scope



\## In Scope



List what is included in this work package.



```text

In Scope:



\- TBD

```



\## Out of Scope



List what is explicitly excluded.



```text

Out of Scope:



\- TBD

```



\---



\# 6. Inputs



List all required input artifacts.



Examples:



\* Constitution

\* AI Organization document

\* Agent Registry

\* RACI Matrix

\* Communication Model

\* Requirement document

\* Previous ADR

\* Test report

\* User request



| Input | Location | Required |

| ----- | -------- | -------- |

| TBD   | TBD      | Yes / No |



\---



\# 7. Expected Outputs



List the required outputs.



Examples:



\* analysis

\* recommendation

\* Markdown document

\* ADR

\* updated backlog entry

\* risk entry

\* review request

\* test case



| Output | Target Location | Required |

| ------ | --------------- | -------- |

| TBD    | TBD             | Yes      |



\---



\# 8. Constraints



List constraints that must be respected.



Examples:



\* must comply with EOS Constitution,

\* must not modify the Constitution,

\* must not make final approval decisions,

\* must use existing templates,

\* must preserve traceability,

\* must escalate safety or compliance uncertainty.



```text

Constraints:



\- TBD

```



\---



\# 9. Required Analysis



The assigned agent shall address the following questions:



```text

Required Analysis:



1\. TBD

2\. TBD

3\. TBD

```



\---



\# 10. Required Response Structure



The assigned agent shall respond using this structure:



```text

1\. Summary

2\. Assumptions

3\. Analysis

4\. Recommendation

5\. Risks

6\. Dependencies

7\. Required Evidence

8\. Open Questions

9\. Documentation Impact

10\. Confidence Level

```



\---



\# 11. Review Requirements



Define whether review is required.



| Review Type                  | Required | Reviewer                      |

| ---------------------------- | -------- | ----------------------------- |

| Orchestrator Review          | Yes / No | Engineering OS Orchestrator   |

| Knowledge Manager Review     | Yes / No | Engineering Knowledge Manager |

| Constitution Guardian Review | Yes / No | Constitution Guardian         |

| Independent Auditor Review   | Yes / No | Independent Auditor           |

| Human Owner Approval         | Yes / No | Human Owner                   |



\---



\# 12. Documentation Requirements



Define what must be documented after completion.



| Documentation Item | Required | Target Location                            |

| ------------------ | -------- | ------------------------------------------ |

| ADR                | Yes / No | `700\_templates/ADR\_TEMPLATE.md`            |

| Backlog Update     | Yes / No | `100\_governance/EOS\_FOUNDATION\_BACKLOG.md` |

| Requirement Update | Yes / No | TBD                                        |

| Risk Update        | Yes / No | TBD                                        |

| Lessons Learned    | Yes / No | `900\_lessons\_learned/`                     |

| Changelog Entry    | Yes / No | `CHANGELOG.md`                             |



\---



\# 13. Acceptance Criteria



The work package is complete when:



\* scope has been addressed,

\* expected outputs have been delivered,

\* assumptions are documented,

\* risks are documented,

\* open questions are listed,

\* required reviews are completed,

\* required documentation updates are identified,

\* Human Owner decision is requested if required.



\---



\# 14. Result



| Field                   | Value                            |

| ----------------------- | -------------------------------- |

| Completion Status       | Open / Done / Blocked / Deferred |

| Completed by            | TBD                              |

| Completion Date         | TBD                              |

| Review Result           | TBD                              |

| Follow-up Work Packages | TBD                              |



\---



\# 15. Change History



| Version | Date | Change                                | Author   |

| ------- | ---- | ------------------------------------- | -------- |

| 0.1     | TBD  | Initial Work Package Request template | EOS Team |



