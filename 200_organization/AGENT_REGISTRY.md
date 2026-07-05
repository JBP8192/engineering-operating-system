\# Agent Registry



\*\*Document ID:\*\* 200-002

\*\*Title:\*\* Agent Registry

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering Knowledge Manager

\*\*Parent Document:\*\* `200\_organization/AI\_ORGANIZATION.md`

\*\*Applies to:\*\* All AI agents within the Engineering Operating System.



\---



\# 1. Purpose



This document is the central registry of all agents within the Engineering Operating System.



It defines:



\* which agents exist,

\* which agents are planned,

\* which agents are active,

\* which agents are deprecated,

\* who owns each agent,

\* which specification belongs to each agent,

\* which prompt implementation belongs to each agent,

\* which priority each agent has,

\* which project or organizational capability each agent supports.



The Agent Registry is the controlled inventory of the AI organization.



No agent shall be considered part of the Engineering Operating System unless it is listed in this registry.



\---



\# 2. Agent Status Model



Each agent shall have exactly one lifecycle status.



| Status     | Meaning                                         |

| ---------- | ----------------------------------------------- |

| Proposed   | Agent idea exists but is not yet specified.     |

| Specified  | Agent role and responsibilities are documented. |

| Prompted   | A first executable prompt exists.               |

| Testing    | Agent is being tested in workflows.             |

| Active     | Agent may be used in normal EOS workflows.      |

| Deprecated | Agent should no longer be used for new work.    |

| Retired    | Agent has been removed from active use.         |



\---



\# 3. Agent Priority Model



Priority describes how important the agent is for the initial EOS setup.



| Priority | Meaning                                                |

| -------- | ------------------------------------------------------ |

| Critical | Required for the EOS to operate safely and coherently. |

| High     | Required for the first useful EOS workflows.           |

| Medium   | Needed soon for product development projects.          |

| Low      | Useful later or only for specific projects.            |



\---



\# 4. Initial Core Agents



| ID   | Agent Name                    | Status    | Version | Priority | Owner       | Specification                                                  | Prompt |

| ---- | ----------------------------- | --------- | ------- | -------- | ----------- | -------------------------------------------------------------- | ------ |

| A000 | Constitution Guardian         | Specified | 0.1     | Critical | Human Owner | `../500\_agent\_specifications/constitution\_guardian.md`         | TBD    |

| A001 | Engineering OS Orchestrator   | Prompted | 0.1     | Critical | Human Owner | `../500\_agent\_specifications/engineering\_os\_orchestrator.md`   | ../prompts/system/core/A001_engineering_os_orchestrator_v0.1.md    |

| A002 | Engineering Knowledge Manager | Prompted | 0.1     | Critical | Human Owner | `../500\_agent\_specifications/engineering\_knowledge\_manager.md` | ../prompts/system/core/A002_engineering_knowledge_manager_v0.1.md    |

| A003 | Chief Systems Engineer        | Proposed  | 0.1     | High     | Human Owner | TBD                                                            | TBD    |

| A004 | Independent Auditor           | Prompted  | 0.1     | High     | Human Owner | TBD                                                            | ../prompts/system/core/A004_independent_auditor_v0.1.md    |



\---



\# 5. Initial Product Development Agents



These agents are expected to be required for the first product project:



`800\_projects/electric-scooter/`



| ID   | Agent Name                      | Status   | Version | Priority | Owner       | Specification | Prompt |

| ---- | ------------------------------- | -------- | ------- | -------- | ----------- | ------------- | ------ |

| A100 | Requirements Engineer           | Proposed | 0.1     | High     | Human Owner | TBD           | TBD    |

| A101 | Homologation \& Compliance Agent | Proposed | 0.1     | High     | Human Owner | TBD           | TBD    |

| A102 | Functional Safety Agent         | Proposed | 0.1     | High     | Human Owner | TBD           | TBD    |

| A103 | Electrical Engineering Agent    | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A104 | Battery \& BMS Agent             | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A105 | Mechanical Engineering Agent    | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A106 | Software / Embedded Agent       | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A107 | Test \& Validation Agent         | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A108 | Supplier Strategy Agent         | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A109 | Cost Engineering Agent          | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A110 | Manufacturing Agent             | Proposed | 0.1     | Low      | Human Owner | TBD           | TBD    |

| A111 | Cybersecurity Agent             | Proposed | 0.1     | Low      | Human Owner | TBD           | TBD    |



\---



\# 6. Tooling and Infrastructure Agents



These agents support operation, automation and tool integration.



| ID   | Agent Name                  | Status   | Version | Priority | Owner       | Specification | Prompt |

| ---- | --------------------------- | -------- | ------- | -------- | ----------- | ------------- | ------ |

| A200 | Tooling Agent               | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A201 | GitHub Repository Manager   | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A202 | OpenClaw Runtime Manager    | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A203 | Telegram Interface Agent    | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A204 | Wiki / Confluence Publisher | Proposed | 0.1     | Low      | Human Owner | TBD           | TBD    |



\---



\# 7. Organizational Learning Agents



These agents support the long-term improvement of the Engineering Operating System itself.



| ID   | Agent Name                      | Status   | Version | Priority | Owner       | Specification | Prompt |

| ---- | ------------------------------- | -------- | ------- | -------- | ----------- | ------------- | ------ |

| A300 | Organizational Learning Manager | Proposed | 0.1     | High     | Human Owner | TBD           | TBD    |

| A301 | Prompt Governance Agent         | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A302 | Workflow Improvement Agent      | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |

| A303 | Lessons Learned Curator         | Proposed | 0.1     | Medium   | Human Owner | TBD           | TBD    |



\---



\# 8. Agent ID Convention



Agent IDs follow this convention:



| Range     | Meaning                                        |

| --------- | ---------------------------------------------- |

| A000–A099 | Core EOS governance and orchestration agents   |

| A100–A199 | Product engineering specialist agents          |

| A200–A299 | Tooling and infrastructure agents              |

| A300–A399 | Organizational learning and improvement agents |

| A400–A499 | Project-specific temporary agents              |

| A900–A999 | Deprecated or retired agents                   |



Agent IDs shall not be reused after retirement.



\---



\# 9. Registry Rules



The following rules apply to this registry:



1\. Every agent must have a unique ID.

2\. Every active agent must have an owner.

3\. Every active agent must have a specification document.

4\. Every active agent must have a prompt implementation.

5\. Every prompt implementation must reference its specification.

6\. No agent may become active without review.

7\. No agent may approve its own activation.

8\. Deprecated agents shall remain listed for traceability.

9\. Retired agents shall not be deleted from the registry.

10\. Changes to this registry shall be documented in the change history.



\---



\# 10. Minimum Activation Criteria



Before an agent can move to `Active`, the following criteria must be met:



\* agent is listed in this registry,

\* role is defined,

\* scope is defined,

\* responsibilities are defined,

\* limits are defined,

\* interfaces are defined,

\* expected outputs are defined,

\* prompt exists,

\* basic test conversation exists,

\* Orchestrator review completed,

\* Knowledge Manager documentation completed,

\* Constitution Guardian review completed if governance-relevant,

\* Human Owner approval completed.



\---



\# 11. Initial Activation Plan



The first activation sequence shall be:



| Order | Agent                           | Reason                                    |

| ----- | ------------------------------- | ----------------------------------------- |

| 1     | Constitution Guardian           | Protects constitutional principles.       |

| 2     | Engineering OS Orchestrator     | Coordinates all later work.               |

| 3     | Engineering Knowledge Manager   | Maintains documentation and traceability. |

| 4     | Independent Auditor             | Enables independent review.               |

| 5     | Chief Systems Engineer          | Enables system-level product development. |

| 6     | Requirements Engineer           | Enables structured product requirements.  |

| 7     | Homologation \& Compliance Agent | Required for regulated products.          |

| 8     | Functional Safety Agent         | Required for safety-relevant systems.     |



\---



\# 12. Open Items



The following items remain open:



\* define exact prompt storage location,

\* define agent testing procedure,

\* define activation review checklist,

\* define agent versioning standard,

\* define prompt versioning standard,

\* define agent performance metrics,

\* define deprecation process,

\* define OpenClaw-specific runtime mapping,

\* define Telegram routing rules.



\---



\# 13. Change History



| Version | Date | Change                          | Author   |

| ------- | ---- | ------------------------------- | -------- |

| 0.1     | TBD  | Initial draft of agent registry | EOS Team |



