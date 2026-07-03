\# Documentation Request Template



\*\*Template ID:\*\* TPL-700-006

\*\*Title:\*\* Documentation Request Template

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering Knowledge Manager

\*\*Related Documents:\*\*



\* `200\_organization/COMMUNICATION\_MODEL.md`

\* `200\_organization/RACI\_MATRIX.md`

\* `100\_governance/AGENT\_ACTIVATION\_CHECKLIST.md`

\* `700\_templates/WORK\_PACKAGE\_REQUEST\_TEMPLATE.md`

\* `700\_templates/REVIEW\_REQUEST\_TEMPLATE.md`



\---



\# 1. Purpose



This template defines the standard structure for requesting documentation updates within the Engineering Operating System.



A Documentation Request is used when a decision, requirement, risk, review result, workflow change, agent change, prompt change, lesson learned or project artifact must be documented in a controlled and traceable way.



The purpose is to ensure that relevant knowledge is not lost in chat history, temporary notes or undocumented decisions.



\---



\# 2. Documentation Request Metadata



| Field                    | Value                                          |

| ------------------------ | ---------------------------------------------- |

| Documentation Request ID | DR-YYYY-NNN                                    |

| Title                    | TBD                                            |

| Created Date             | TBD                                            |

| Requested by             | TBD                                            |

| Assigned to              | Engineering Knowledge Manager                  |

| Priority                 | Low / Medium / High / Critical                 |

| Risk Class               | C0 / C1 / C2 / C3 / C4 / C5 / C6               |

| Status                   | Open / In Progress / Done / Blocked / Deferred |

| Related Project          | TBD                                            |

| Related Work Package     | TBD                                            |

| Related Review Request   | TBD                                            |

| Related Decision         | TBD                                            |



\---



\# 3. Documentation Trigger



Select the reason why documentation is required.



| Trigger                          | Applies  |

| -------------------------------- | -------- |

| New requirement                  | Yes / No |

| Changed requirement              | Yes / No |

| New architecture decision        | Yes / No |

| Changed architecture decision    | Yes / No |

| New risk                         | Yes / No |

| Changed risk                     | Yes / No |

| New agent                        | Yes / No |

| Changed agent                    | Yes / No |

| Prompt change                    | Yes / No |

| Workflow change                  | Yes / No |

| Tool configuration change        | Yes / No |

| Review result                    | Yes / No |

| Test result                      | Yes / No |

| Project milestone                | Yes / No |

| Lesson learned                   | Yes / No |

| Open issue / unresolved decision | Yes / No |

| Other                            | TBD      |



\---



\# 4. Context



Describe why this documentation update is needed.



Include:



\* what happened,

\* who requested it,

\* which decision or artifact triggered it,

\* what would be lost if it is not documented,

\* which documents are affected.



```text

Context:



TBD

```



\---



\# 5. Information to Document



Describe the information that must be captured.



```text

Information to Document:



TBD

```



\---



\# 6. Target Documentation Type



Select the target documentation type.



| Documentation Type     | Applies  | Target Location |

| ---------------------- | -------- | --------------- |

| ADR                    | Yes / No | TBD             |

| Requirement            | Yes / No | TBD             |

| Risk                   | Yes / No | TBD             |

| Agent Specification    | Yes / No | TBD             |

| Prompt                 | Yes / No | TBD             |

| Workflow               | Yes / No | TBD             |

| Review Report          | Yes / No | TBD             |

| Test Report            | Yes / No | TBD             |

| Backlog Entry          | Yes / No | TBD             |

| Lessons Learned        | Yes / No | TBD             |

| Changelog Entry        | Yes / No | `CHANGELOG.md`  |

| Wiki / Confluence Page | Yes / No | TBD             |

| Other                  | Yes / No | TBD             |



\---



\# 7. Source of Truth



Define where the final authoritative information shall live.



| Information Type      | Source of Truth               |

| --------------------- | ----------------------------- |

| Constitution          | GitHub                        |

| Governance document   | GitHub                        |

| Organization document | GitHub                        |

| Agent specification   | GitHub                        |

| Prompt                | GitHub                        |

| Workflow              | GitHub                        |

| ADR                   | GitHub                        |

| Requirement           | GitHub or requirements system |

| Risk                  | GitHub or risk register       |

| Review report         | GitHub                        |

| Test report           | GitHub                        |

| Lessons learned       | GitHub                        |

| Wiki explanation      | Wiki / Confluence             |

| Temporary discussion  | Telegram / OpenClaw           |



If information exists in multiple places, the defined source of truth prevails.



\---



\# 8. Affected Artifacts



List all artifacts that may need to be created or updated.



| Artifact | Location | Action                                   |

| -------- | -------- | ---------------------------------------- |

| TBD      | TBD      | Create / Update / Review / Delete / Link |



\---



\# 9. Traceability Links



List all related items.



| Link Type    | Reference |

| ------------ | --------- |

| Requirement  | TBD       |

| ADR          | TBD       |

| Risk         | TBD       |

| Test         | TBD       |

| Review       | TBD       |

| Work Package | TBD       |

| Backlog Item | TBD       |

| Agent        | TBD       |

| Prompt       | TBD       |

| Project      | TBD       |



\---



\# 10. Required Documentation Action



The Engineering Knowledge Manager shall perform the following action:



```text

Required Action:



\- TBD

```



Possible actions:



\* create new document,

\* update existing document,

\* create ADR,

\* update Agent Registry,

\* update Foundation Backlog,

\* update changelog,

\* add traceability links,

\* create lesson learned,

\* prepare Wiki summary,

\* request review.



\---



\# 11. Review Requirements



Define whether the documentation update requires review.



| Review Type                  | Required | Reviewer                      |

| ---------------------------- | -------- | ----------------------------- |

| Knowledge Manager self-check | Yes      | Engineering Knowledge Manager |

| Orchestrator Review          | Yes / No | Engineering OS Orchestrator   |

| Constitution Guardian Review | Yes / No | Constitution Guardian         |

| Independent Auditor Review   | Yes / No | Independent Auditor           |

| Human Owner Approval         | Yes / No | Human Owner                   |



Review is required when documentation changes affect:



\* Constitution,

\* governance,

\* agent authority,

\* prompt behavior,

\* safety,

\* compliance,

\* architecture baselines,

\* decision records,

\* source-of-truth structure.



\---



\# 12. Acceptance Criteria



The documentation request is complete when:



\* target artifact has been created or updated,

\* information is placed in the correct source of truth,

\* affected artifacts are linked,

\* assumptions are documented,

\* open questions are documented,

\* required reviews are completed,

\* changelog is updated if required,

\* backlog is updated if required,

\* no important decision remains only in chat history.



\---



\# 13. Result



| Field             | Value                            |

| ----------------- | -------------------------------- |

| Completion Status | Open / Done / Blocked / Deferred |

| Completed by      | TBD                              |

| Completion Date   | TBD                              |

| Updated Artifacts | TBD                              |

| Review Result     | TBD                              |

| Follow-up Actions | TBD                              |



\---



\# 14. Documentation Quality Checklist



| Check                                     |      Required | Status |

| ----------------------------------------- | ------------: | ------ |

| Clear title                               |           Yes | TBD    |

| Clear owner                               |           Yes | TBD    |

| Version defined                           |           Yes | TBD    |

| Status defined                            |           Yes | TBD    |

| Related documents linked                  |           Yes | TBD    |

| Decision rationale captured if applicable | If applicable | TBD    |

| Alternatives captured if applicable       | If applicable | TBD    |

| Risks captured if applicable              | If applicable | TBD    |

| Open questions captured if applicable     | If applicable | TBD    |

| Source of truth clear                     |           Yes | TBD    |

| Changelog updated if required             | If applicable | TBD    |

| Backlog updated if required               | If applicable | TBD    |



\---



\# 15. Documentation Anti-Patterns



The following patterns are not allowed:



1\. Important decisions remaining only in chat.

2\. Multiple conflicting sources of truth.

3\. Updating Wiki pages without updating GitHub source artifacts.

4\. Closing documentation tasks without evidence.

5\. Deleting open items without traceability.

6\. Creating new documents without linking them.

7\. Documenting conclusions without assumptions.

8\. Documenting architecture decisions without rationale.

9\. Treating Telegram as permanent documentation.

10\. Treating undocumented decisions as stable.



\---



\# 16. Change History



| Version | Date | Change                                 | Author   |

| ------- | ---- | -------------------------------------- | -------- |

| 0.1     | TBD  | Initial Documentation Request template | EOS Team |



