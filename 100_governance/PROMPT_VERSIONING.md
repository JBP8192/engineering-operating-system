\# Prompt Versioning



\*\*Document ID:\*\* 100-002

\*\*Title:\*\* Prompt Versioning

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering Knowledge Manager

\*\*Parent Documents:\*\*



\* `000\_constitution/EOSC\_v0.1.md`

\* `200\_organization/AI\_ORGANIZATION.md`

\* `200\_organization/AGENT\_REGISTRY.md`

\* `prompts/README.md`



\---



\# 1. Purpose



This document defines how prompt implementations are versioned, reviewed, released and deprecated within the Engineering Operating System.



The purpose is to prevent uncontrolled prompt changes and to ensure that agent behavior remains traceable, reviewable and aligned with the EOS Constitution.



A prompt is not just text.



A prompt is an executable implementation of an agent specification.



Therefore, prompt changes are treated as controlled configuration changes.



\---



\# 2. Core Principle



Agent specifications define what an agent is.



Prompts define how an agent is currently implemented.



The specification is the role definition.



The prompt is the executable behavior.



No prompt may extend the authority of an agent beyond its specification.



No prompt may contradict the EOS Constitution.



\---



\# 3. Prompt Storage Location



Executable prompts are stored in:



`prompts/`



Core agent prompts are stored in:



`prompts/system/core/`



Specialist agent prompts are stored in:



`prompts/system/specialists/`



Prompt tests are stored in:



`prompts/tests/`



\---



\# 4. Prompt Naming Convention



Prompt files shall use the following naming convention:



```text

<agent\_id>\_<agent\_name>\_v<major>.<minor>.md

```



Example:



```text

A001\_engineering\_os\_orchestrator\_v0.1.md

A002\_engineering\_knowledge\_manager\_v0.1.md

A000\_constitution\_guardian\_v0.1.md

```



Prompt test files shall use:



```text

<agent\_id>\_<agent\_name>\_test\_v<major>.<minor>.md

```



Example:



```text

A001\_engineering\_os\_orchestrator\_test\_v0.1.md

```



\---



\# 5. Version Numbering



Prompts use semantic versioning:



```text

MAJOR.MINOR.PATCH

```



During the foundation phase, `MAJOR.MINOR` is sufficient.



\## Major Version



Increment the major version when:



\* the agent’s authority changes,

\* the agent’s core mission changes,

\* the agent’s decision behavior changes,

\* tool access changes significantly,

\* safety, governance or compliance behavior changes.



Example:



```text

v1.0 → v2.0

```



\## Minor Version



Increment the minor version when:



\* response format is improved,

\* additional checks are added,

\* instructions are clarified,

\* new non-critical behavior is added,

\* documentation behavior is improved.



Example:



```text

v0.1 → v0.2

```



\## Patch Version



Increment the patch version when:



\* typos are fixed,

\* formatting is improved,

\* wording is clarified without behavior change,

\* broken references are corrected.



Example:



```text

v1.0.0 → v1.0.1

```



\---



\# 6. Prompt Header



Every prompt file shall begin with a metadata header.



Required fields:



```markdown

\# <Agent Name> System Prompt



\*\*Agent ID:\*\* Axxx  

\*\*Prompt Version:\*\* v0.1  

\*\*Status:\*\* Draft  

\*\*Owner:\*\* Engineering Knowledge Manager  

\*\*Specification:\*\* `../../500\_agent\_specifications/<agent>.md`  

\*\*Registry:\*\* `../../200\_organization/AGENT\_REGISTRY.md`  

\*\*Constitution:\*\* `../../000\_constitution/EOSC\_v0.1.md`  

```



\---



\# 7. Prompt Status Model



| Status     | Meaning                                       |

| ---------- | --------------------------------------------- |

| Draft      | Prompt is being written.                      |

| Review     | Prompt is ready for review.                   |

| Testing    | Prompt is being tested.                       |

| Active     | Prompt may be used in normal EOS workflows.   |

| Deprecated | Prompt should no longer be used for new work. |

| Retired    | Prompt has been removed from active use.      |



Only prompts with status `Active` may be used as official EOS agents.



\---



\# 8. Prompt Change Requirements



Every prompt change shall include:



\* reason for change,

\* affected agent,

\* affected specification,

\* expected behavior change,

\* risk assessment,

\* review requirement,

\* changelog entry.



Prompt changes shall be committed to Git.



Prompt changes affecting governance, decision authority, safety, compliance or tool permissions require review.



\---



\# 9. Review Requirements



\## Low-risk prompt changes



Examples:



\* formatting,

\* typo correction,

\* wording clarification,

\* broken link correction.



Required review:



\* Engineering Knowledge Manager



\## Medium-risk prompt changes



Examples:



\* new output format,

\* improved workflow behavior,

\* additional documentation rules,

\* new escalation rule.



Required review:



\* Engineering Knowledge Manager

\* Engineering OS Orchestrator



\## High-risk prompt changes



Examples:



\* changed decision authority,

\* new tool access,

\* changed safety behavior,

\* changed compliance behavior,

\* changed governance behavior.



Required review:



\* Engineering OS Orchestrator

\* Constitution Guardian

\* Independent Auditor

\* Human Owner approval



\---



\# 10. Activation Criteria



A prompt may become active only when:



\* agent is listed in `AGENT\_REGISTRY.md`,

\* agent specification exists,

\* prompt file exists,

\* prompt references specification,

\* prompt references Constitution,

\* prompt status is set to `Review` or `Testing`,

\* basic test conversation exists,

\* review requirements are met,

\* activation checklist is completed,

\* Human Owner approves activation.



\---



\# 11. Deprecated Prompts



Deprecated prompts shall not be deleted immediately.



They shall remain available for traceability.



A deprecated prompt shall include:



\* replacement prompt,

\* reason for deprecation,

\* date of deprecation,

\* migration note.



\---



\# 12. Prompt Change History



Every prompt file shall contain a change history section.



Example:



```markdown

\# Change History



| Version | Date | Change | Author |

|---|---|---|---|

| 0.1 | TBD | Initial draft | EOS Team |

```



\---



\# 13. Open Items



Open items for this document are tracked centrally in:



`EOS\_FOUNDATION\_BACKLOG.md`



This document shall not be used as an active task list.



\---



\# 14. Change History



| Version | Date | Change                             | Author   |

| ------- | ---- | ---------------------------------- | -------- |

| 0.1     | TBD  | Initial prompt versioning standard | EOS Team |



