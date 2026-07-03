\# Agent Activation Record Template



\*\*Template ID:\*\* TPL-700-008

\*\*Title:\*\* Agent Activation Record Template

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering OS Orchestrator

\*\*Related Documents:\*\*



\* `100\_governance/AGENT\_ACTIVATION\_CHECKLIST.md`

\* `100\_governance/AGENT\_TESTING\_PROCEDURE.md`

\* `100\_governance/PROMPT\_VERSIONING.md`

\* `200\_organization/AGENT\_REGISTRY.md`

\* `700\_templates/AGENT\_TEST\_REPORT\_TEMPLATE.md`



\---



\# 1. Purpose



This template defines the standard record used to document the activation of an AI agent within the Engineering Operating System.



An Agent Activation Record confirms that an agent has passed the required preparation, review and testing steps and may be used in official EOS workflows.



The purpose is to make agent activation traceable, reviewable and reversible.



\---



\# 2. Activation Record Metadata



| Field                        | Value                                                     |

| ---------------------------- | --------------------------------------------------------- |

| Activation Record ID         | AAR-YYYY-NNN                                              |

| Agent ID                     | TBD                                                       |

| Agent Name                   | TBD                                                       |

| Agent Type                   | Core / Specialist / Tooling / Learning                    |

| Activation Date              | TBD                                                       |

| Activation Status            | Approved / Approved with Conditions / Rejected / Deferred |

| Approved by                  | Human Owner                                               |

| Prepared by                  | Engineering OS Orchestrator                               |

| Documented by                | Engineering Knowledge Manager                             |

| Reviewed by                  | Independent Auditor / Constitution Guardian if applicable |

| Related Test Report          | TBD                                                       |

| Related Activation Checklist | TBD                                                       |



\---



\# 3. Agent Identification



| Field                 | Value                                   |

| --------------------- | --------------------------------------- |

| Agent ID              | TBD                                     |

| Agent Name            | TBD                                     |

| Registry Entry        | `200\_organization/AGENT\_REGISTRY.md`    |

| Agent Specification   | TBD                                     |

| Prompt File           | TBD                                     |

| Prompt Version        | TBD                                     |

| Specification Version | TBD                                     |

| Owner                 | TBD                                     |

| Runtime               | OpenClaw / ChatGPT / Local / Other      |

| Interface             | Telegram / OpenClaw UI / GitHub / Other |



\---



\# 4. Activation Scope



Describe what the agent is allowed to do after activation.



```text

Activation Scope:



TBD

```



Examples:



\* may route user requests,

\* may create work packages,

\* may propose documentation updates,

\* may draft ADRs,

\* may review artifacts,

\* may answer within its specialist domain,

\* may use selected tools,

\* may update repository files only after approval.



\---



\# 5. Explicit Limits



Describe what the agent is not allowed to do.



```text

Explicit Limits:



\- TBD

```



Common limits:



\* may not approve its own work as final,

\* may not override the Human Owner,

\* may not change the Constitution,

\* may not modify prompts without documentation,

\* may not make final safety decisions,

\* may not make final regulatory conclusions,

\* may not make financial commitments,

\* may not bypass review requirements.



\---



\# 6. Activation Preconditions



| Precondition                     | Required | Status | Evidence |

| -------------------------------- | -------: | ------ | -------- |

| Agent listed in Agent Registry   |      Yes | TBD    | TBD      |

| Agent specification exists       |      Yes | TBD    | TBD      |

| Prompt implementation exists     |      Yes | TBD    | TBD      |

| Prompt version defined           |      Yes | TBD    | TBD      |

| Prompt follows naming convention |      Yes | TBD    | TBD      |

| Prompt references Constitution   |      Yes | TBD    | TBD      |

| Prompt references specification  |      Yes | TBD    | TBD      |

| Activation checklist completed   |      Yes | TBD    | TBD      |

| Test report completed            |      Yes | TBD    | TBD      |

| Review completed                 |      Yes | TBD    | TBD      |

| Human Owner approval obtained    |      Yes | TBD    | TBD      |



\---



\# 7. Test Summary



| Field                    | Value                                               |

| ------------------------ | --------------------------------------------------- |

| Test Report              | TBD                                                 |

| Test Status              | Passed / Passed with Conditions / Failed / Deferred |

| Number of Test Scenarios | TBD                                                 |

| Blocker Findings         | TBD                                                 |

| Major Findings           | TBD                                                 |

| Minor Findings           | TBD                                                 |

| Remaining Conditions     | TBD                                                 |



```text

Test Summary:



TBD

```



\---



\# 8. Review Summary



| Review Type                          |      Required | Result | Reviewer |

| ------------------------------------ | ------------: | ------ | -------- |

| Engineering Knowledge Manager Review |           Yes | TBD    | TBD      |

| Engineering OS Orchestrator Review   |           Yes | TBD    | TBD      |

| Constitution Guardian Review         | If applicable | TBD    | TBD      |

| Independent Auditor Review           | If applicable | TBD    | TBD      |

| Human Owner Approval                 |           Yes | TBD    | TBD      |



```text

Review Summary:



TBD

```



\---



\# 9. Activation Decision



Select one activation result.



| Result                   | Applies  |

| ------------------------ | -------- |

| Approved                 | Yes / No |

| Approved with Conditions | Yes / No |

| Rejected                 | Yes / No |

| Deferred                 | Yes / No |



\## Decision Rationale



```text

Decision Rationale:



TBD

```



\---



\# 10. Conditions and Restrictions



If the activation is approved with conditions, list all restrictions.



| Condition ID | Condition | Owner | Required Until | Status |

| ------------ | --------- | ----- | -------------- | ------ |

| C-001        | TBD       | TBD   | TBD            | Open   |



Examples:



\* agent may only be used in draft mode,

\* agent may not modify repository files,

\* agent may not handle safety-related requests,

\* agent output requires Orchestrator review,

\* agent may only operate through Telegram,

\* agent may not use external tools.



\---



\# 11. Tool Access



| Tool              | Access Level                  | Allowed Actions | Forbidden Actions | Human Approval Required |

| ----------------- | ----------------------------- | --------------- | ----------------- | ----------------------- |

| GitHub            | None / Read / Write           | TBD             | TBD               | Yes / No                |

| OpenClaw          | None / Runtime / Admin        | TBD             | TBD               | Yes / No                |

| Telegram          | None / Read / Send            | TBD             | TBD               | Yes / No                |

| Wiki / Confluence | None / Read / Draft / Publish | TBD             | TBD               | Yes / No                |

| Local Files       | None / Read / Write           | TBD             | TBD               | Yes / No                |



\---



\# 12. Monitoring Requirements



Define how the agent shall be monitored after activation.



| Monitoring Item                   |          Required | Owner                      | Frequency |

| --------------------------------- | ----------------: | -------------------------- | --------- |

| Output quality review             |               Yes | Orchestrator               | TBD       |

| Governance behavior review        |     If applicable | Constitution Guardian      | TBD       |

| Documentation completeness review |     If applicable | Knowledge Manager          | TBD       |

| Test regression review            | If prompt changes | Independent Auditor        | TBD       |

| Human feedback review             |               Yes | Human Owner / Orchestrator | TBD       |



\---



\# 13. Rollback Plan



Define how the agent can be deactivated or rolled back.



```text

Rollback Plan:



TBD

```



Minimum rollback requirements:



\* mark agent as Deprecated or Retired in Agent Registry,

\* deactivate prompt in runtime,

\* document reason,

\* preserve previous prompt version,

\* create follow-up backlog item,

\* capture lesson learned if needed.



\---



\# 14. Follow-up Actions



| Action ID | Action | Owner | Priority | Required Before | Status |

| --------- | ------ | ----- | -------- | --------------- | ------ |

| A-001     | TBD    | TBD   | TBD      | TBD             | Open   |



\---



\# 15. Documentation Impact



| Documentation Item          |      Required | Target Location                                | Status |

| --------------------------- | ------------: | ---------------------------------------------- | ------ |

| Agent Registry Update       |           Yes | `200\_organization/AGENT\_REGISTRY.md`           | TBD    |

| Activation Checklist Update |           Yes | `100\_governance/AGENT\_ACTIVATION\_CHECKLIST.md` | TBD    |

| Test Report Link            |           Yes | `prompts/tests/`                               | TBD    |

| Changelog Update            |           Yes | `CHANGELOG.md`                                 | TBD    |

| Backlog Update              | If applicable | `100\_governance/EOS\_FOUNDATION\_BACKLOG.md`     | TBD    |

| Lessons Learned             | If applicable | `900\_lessons\_learned/`                         | TBD    |



\---



\# 16. Approval



| Role                              | Name | Decision                                                  | Date |

| --------------------------------- | ---- | --------------------------------------------------------- | ---- |

| Engineering OS Orchestrator       | TBD  | Recommend / Do not recommend                              | TBD  |

| Engineering Knowledge Manager     | TBD  | Documentation complete / incomplete                       | TBD  |

| Constitution Guardian if required | TBD  | Aligned / Not aligned                                     | TBD  |

| Independent Auditor if required   | TBD  | Accepted / Rejected / Deferred                            | TBD  |

| Human Owner                       | TBD  | Approved / Approved with Conditions / Rejected / Deferred | TBD  |



\---



\# 17. Activation Statement



```text

Activation Statement:



The agent listed in this record has been reviewed according to the defined activation process.



Activation result:



TBD



Restrictions:



TBD



The agent may only operate within the scope and limits documented in this record.

```



\---



\# 18. Change History



| Version | Date | Change                                   | Author   |

| ------- | ---- | ---------------------------------------- | -------- |

| 0.1     | TBD  | Initial Agent Activation Record template | EOS Team |



