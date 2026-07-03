\# Agent Activation Checklist



\*\*Document ID:\*\* 100-003

\*\*Title:\*\* Agent Activation Checklist

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering OS Orchestrator

\*\*Parent Documents:\*\*



\* `000\_constitution/EOSC\_v0.1.md`

\* `100\_governance/PROMPT\_VERSIONING.md`

\* `200\_organization/AI\_ORGANIZATION.md`

\* `200\_organization/AGENT\_REGISTRY.md`

\* `200\_organization/RACI\_MATRIX.md`

\* `200\_organization/COMMUNICATION\_MODEL.md`



\---



\# 1. Purpose



This document defines the checklist that must be completed before an AI agent can be activated within the Engineering Operating System.



The purpose is to prevent uncontrolled agent activation, unclear responsibilities, unreviewed prompts and undocumented behavior.



An agent may only become active when its role, scope, prompt, tests, interfaces and governance alignment have been checked.



\---



\# 2. Core Principle



No agent shall be activated only because a prompt exists.



An agent is active only when:



\* it is listed in the Agent Registry,

\* its specification exists,

\* its prompt implementation exists,

\* its responsibilities are clear,

\* its limits are clear,

\* its interfaces are defined,

\* its output format is defined,

\* its tests are completed,

\* required reviews are completed,

\* activation is approved by the Human Owner.



\---



\# 3. Activation Status



The activation checklist supports the agent lifecycle defined in the Agent Registry.



```text

Proposed

&#x20;   ↓

Specified

&#x20;   ↓

Prompted

&#x20;   ↓

Testing

&#x20;   ↓

Active

&#x20;   ↓

Deprecated

&#x20;   ↓

Retired

```



Only agents with status `Active` may be used in official EOS workflows.



\---



\# 4. Required Activation Checklist



\## 4.1 Registry Check



| Check                                                    | Required | Status |

| -------------------------------------------------------- | -------: | ------ |

| Agent has a unique Agent ID.                             |      Yes | TBD    |

| Agent is listed in `200\_organization/AGENT\_REGISTRY.md`. |      Yes | TBD    |

| Agent has an assigned owner.                             |      Yes | TBD    |

| Agent has a defined lifecycle status.                    |      Yes | TBD    |

| Agent has a priority classification.                     |      Yes | TBD    |

| Agent has links to specification and prompt files.       |      Yes | TBD    |



\---



\## 4.2 Specification Check



| Check                                                      | Required | Status |

| ---------------------------------------------------------- | -------: | ------ |

| Agent specification exists in `500\_agent\_specifications/`. |      Yes | TBD    |

| Mission is defined.                                        |      Yes | TBD    |

| Scope is defined.                                          |      Yes | TBD    |

| Responsibilities are defined.                              |      Yes | TBD    |

| Explicit limits are defined.                               |      Yes | TBD    |

| Inputs are defined.                                        |      Yes | TBD    |

| Outputs are defined.                                       |      Yes | TBD    |

| Interfaces to other agents are defined.                    |      Yes | TBD    |

| Escalation rules are defined.                              |      Yes | TBD    |

| Review requirements are defined.                           |      Yes | TBD    |

| Agent does not conflict with existing agents.              |      Yes | TBD    |



\---



\## 4.3 Prompt Check



| Check                                                      | Required | Status |

| ---------------------------------------------------------- | -------: | ------ |

| Prompt file exists in `prompts/`.                          |      Yes | TBD    |

| Prompt follows naming convention.                          |      Yes | TBD    |

| Prompt includes metadata header.                           |      Yes | TBD    |

| Prompt references the agent specification.                 |      Yes | TBD    |

| Prompt references the EOS Constitution.                    |      Yes | TBD    |

| Prompt version is defined.                                 |      Yes | TBD    |

| Prompt status is defined.                                  |      Yes | TBD    |

| Prompt does not extend authority beyond the specification. |      Yes | TBD    |

| Prompt does not contradict the Constitution.               |      Yes | TBD    |

| Prompt includes expected response structure.               |      Yes | TBD    |

| Prompt includes uncertainty handling rules.                |      Yes | TBD    |

| Prompt includes escalation behavior.                       |      Yes | TBD    |

| Prompt includes documentation triggers if applicable.      |      Yes | TBD    |

| Prompt includes change history.                            |      Yes | TBD    |



\---



\## 4.4 Governance Check



| Check                                                                        |      Required | Status |

| ---------------------------------------------------------------------------- | ------------: | ------ |

| Agent aligns with the Constitution.                                          |           Yes | TBD    |

| Agent respects human final decision authority.                               |           Yes | TBD    |

| Agent does not approve its own work as final.                                |           Yes | TBD    |

| Agent follows the communication model.                                       |           Yes | TBD    |

| Agent follows the RACI matrix.                                               |           Yes | TBD    |

| Agent has no uncontrolled tool authority.                                    |           Yes | TBD    |

| Agent has defined escalation paths.                                          |           Yes | TBD    |

| Governance-relevant behavior has been reviewed by the Constitution Guardian. | If applicable | TBD    |



\---



\## 4.5 Tool Access Check



| Check                                              |      Required | Status |

| -------------------------------------------------- | ------------: | ------ |

| Required tools are listed.                         |           Yes | TBD    |

| Forbidden tools or actions are listed.             | If applicable | TBD    |

| Tool access is limited to the agent’s scope.       |           Yes | TBD    |

| Tool permissions are documented.                   |           Yes | TBD    |

| Tool output handling is defined.                   |           Yes | TBD    |

| Tool failures are handled safely.                  |           Yes | TBD    |

| Tool actions requiring human approval are defined. |           Yes | TBD    |



\---



\## 4.6 Test Check



| Check                                                   |      Required | Status |

| ------------------------------------------------------- | ------------: | ------ |

| Basic test conversation exists in `prompts/tests/`.     |           Yes | TBD    |

| Expected behavior is documented.                        |           Yes | TBD    |

| Out-of-scope behavior is tested.                        |           Yes | TBD    |

| Escalation behavior is tested.                          |           Yes | TBD    |

| Uncertainty handling is tested.                         |           Yes | TBD    |

| Documentation trigger behavior is tested if applicable. | If applicable | TBD    |

| Governance conflict behavior is tested if applicable.   | If applicable | TBD    |

| Test result is documented.                              |           Yes | TBD    |



\---



\## 4.7 Review Check



| Check                                           |               Required | Status |

| ----------------------------------------------- | ---------------------: | ------ |

| Engineering Knowledge Manager review completed. |                    Yes | TBD    |

| Engineering OS Orchestrator review completed.   |                    Yes | TBD    |

| Constitution Guardian review completed.         | If governance-relevant | TBD    |

| Independent Auditor review completed.           |           If high-risk | TBD    |

| Human Owner approval completed.                 |                    Yes | TBD    |



\---



\## 4.8 Documentation Check



| Check                           | Required | Status |

| ------------------------------- | -------: | ------ |

| Agent Registry updated.         |      Yes | TBD    |

| Agent specification committed.  |      Yes | TBD    |

| Prompt committed.               |      Yes | TBD    |

| Prompt tests committed.         |      Yes | TBD    |

| Relevant changelog updated.     |      Yes | TBD    |

| Related backlog items updated.  |      Yes | TBD    |

| Activation decision documented. |      Yes | TBD    |



\---



\# 5. Activation Decision



An agent activation decision shall include:



| Field                     | Value |

| ------------------------- | ----- |

| Agent ID                  | TBD   |

| Agent Name                | TBD   |

| Prompt Version            | TBD   |

| Specification Version     | TBD   |

| Activation Status         | TBD   |

| Activation Date           | TBD   |

| Approved by               | TBD   |

| Conditions / Restrictions | TBD   |

| Follow-up Actions         | TBD   |



\---



\# 6. Activation Result



The final activation result shall be one of:



| Result                   | Meaning                                           |

| ------------------------ | ------------------------------------------------- |

| Approved                 | Agent may be used in official EOS workflows.      |

| Approved with Conditions | Agent may be used only under listed restrictions. |

| Rejected                 | Agent may not be activated. Rework required.      |

| Deferred                 | Activation postponed. Reason must be documented.  |



\---



\# 7. Minimum Checklist for First EOS Agents



For the initial foundation phase, the following minimum checklist must be completed for:



\* A000 Constitution Guardian

\* A001 Engineering OS Orchestrator

\* A002 Engineering Knowledge Manager

\* A004 Independent Auditor



Minimum required items:



\* registry entry,

\* agent specification,

\* prompt implementation,

\* prompt version,

\* basic test case,

\* governance review,

\* activation decision,

\* documentation update.



\---



\# 8. Fast-Track Activation



Fast-track activation may be used only for low-risk, non-governance, non-safety and non-regulatory helper agents.



Fast-track activation shall not be used for:



\* Constitution Guardian,

\* Engineering OS Orchestrator,

\* Engineering Knowledge Manager,

\* Independent Auditor,

\* Functional Safety Agent,

\* Compliance Agent,

\* agents with write access to repositories,

\* agents with tool execution authority,

\* agents that influence safety, compliance or architecture decisions.



\---



\# 9. Deactivation and Rollback



If an active agent behaves outside its defined scope, it may be deactivated.



Deactivation reasons include:



\* governance violation,

\* repeated incorrect routing,

\* undocumented tool usage,

\* unsafe recommendations,

\* conflicting responsibilities,

\* prompt behavior inconsistent with specification,

\* human owner decision.



A deactivation shall be documented in:



\* Agent Registry,

\* Change History,

\* relevant backlog item,

\* lessons learned if applicable.



\---



\# 10. Open Items



Open items for this document are tracked centrally in:



`EOS\_FOUNDATION\_BACKLOG.md`



This document shall not be used as an active task list.



\---



\# 11. Change History



| Version | Date | Change                             | Author   |

| ------- | ---- | ---------------------------------- | -------- |

| 0.1     | TBD  | Initial agent activation checklist | EOS Team |



