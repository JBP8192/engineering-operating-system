\# RACI Matrix



\*\*Document ID:\*\* 200-003

\*\*Title:\*\* RACI Matrix

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering OS Orchestrator

\*\*Parent Document:\*\* `200\_organization/AI\_ORGANIZATION.md`

\*\*Applies to:\*\* All agents, workflows, tools and projects within the Engineering Operating System.



\---



\# 1. Purpose



This document defines responsibility assignments within the Engineering Operating System using the RACI model.



The purpose is to make clear who performs work, who owns the outcome, who must be consulted and who must be informed.



The RACI Matrix prevents unclear ownership, duplicated work, hidden approval paths and uncontrolled agent autonomy.



\---



\# 2. RACI Definitions



| Letter | Meaning     | Description                                                              |

| ------ | ----------- | ------------------------------------------------------------------------ |

| R      | Responsible | Performs the work or prepares the artifact.                              |

| A      | Accountable | Owns the final outcome or decision. Only one role should be accountable. |

| C      | Consulted   | Provides input before the decision or artifact is finalized.             |

| I      | Informed    | Must be informed after progress, change or decision.                     |



\---



\# 3. General Rules



1\. Every important activity shall have exactly one accountable role.

2\. A role may be responsible without being accountable.

3\. No agent may be accountable for final human decisions.

4\. No agent may independently approve its own work as final.

5\. Safety-relevant, regulatory, financial and constitutional decisions require human accountability.

6\. Documentation-relevant activities shall involve the Engineering Knowledge Manager.

7\. Governance-relevant activities shall involve the Constitution Guardian.

8\. Review-relevant activities shall involve the Independent Auditor.

9\. The Orchestrator coordinates work but does not replace specialist ownership.

10\. If ownership is unclear, the issue shall be escalated to the Human Owner.



\---



\# 4. Core Roles



The following roles are used in this matrix.



| Abbreviation | Role                            |

| ------------ | ------------------------------- |

| HO           | Human Owner                     |

| CG           | Constitution Guardian           |

| ORCH         | Engineering OS Orchestrator     |

| KM           | Engineering Knowledge Manager   |

| CSE          | Chief Systems Engineer          |

| AUD          | Independent Auditor             |

| REQ          | Requirements Engineer           |

| COMP         | Homologation \& Compliance Agent |

| SAFE         | Functional Safety Agent         |

| EE           | Electrical Engineering Agent    |

| BMS          | Battery \& BMS Agent             |

| ME           | Mechanical Engineering Agent    |

| SW           | Software / Embedded Agent       |

| TEST         | Test \& Validation Agent         |

| COST         | Cost Engineering Agent          |

| SUP          | Supplier Strategy Agent         |

| TOOL         | Tooling Agent                   |



\---



\# 5. EOS Governance RACI



| Activity                               | HO | CG  | ORCH | KM | AUD |

| -------------------------------------- | -- | --- | ---- | -- | --- |

| Maintain Constitution                  | A  | R/C | C    | R  | C   |

| Propose Constitution change            | A  | C   | R    | R  | C   |

| Approve Constitution change            | A  | C   | C    | I  | C   |

| Maintain AI Organization document      | A  | C   | R    | R  | C   |

| Maintain Agent Registry                | A  | C   | C    | R  | I   |

| Maintain RACI Matrix                   | A  | C   | R    | R  | C   |

| Define agent lifecycle                 | A  | C   | R    | R  | C   |

| Approve new agent                      | A  | C   | R    | C  | C   |

| Retire agent                           | A  | C   | R    | R  | C   |

| Define organizational release          | A  | C   | R    | R  | C   |

| Capture organizational lessons learned | I  | C   | C    | R  | I   |



\---



\# 6. Agent Development RACI



| Activity                               | HO | CG | ORCH | KM | AUD |

| -------------------------------------- | -- | -- | ---- | -- | --- |

| Propose new agent                      | A  | C  | R    | C  | I   |

| Define agent mission                   | A  | C  | R    | R  | C   |

| Define agent scope and limits          | A  | C  | R    | R  | C   |

| Create agent specification             | A  | C  | C    | R  | C   |

| Create system prompt                   | A  | C  | C    | R  | C   |

| Review prompt for governance alignment | A  | R  | C    | C  | C   |

| Test agent behavior                    | A  | C  | R    | C  | C   |

| Approve agent activation               | A  | C  | R    | C  | C   |

| Monitor agent performance              | I  | C  | R    | R  | C   |

| Update agent prompt                    | A  | C  | C    | R  | C   |

| Deprecate agent                        | A  | C  | R    | R  | C   |



\---



\# 7. Project Start RACI



| Activity                   | HO | ORCH | KM | CSE | REQ | COMP | SAFE | AUD |

| -------------------------- | -- | ---- | -- | --- | --- | ---- | ---- | --- |

| Define project idea        | A  | R    | I  | C   | C   | C    | C    | I   |

| Create project folder      | A  | C    | R  | I   | I   | I    | I    | I   |

| Create project charter     | A  | R    | R  | C   | C   | C    | C    | C   |

| Define project objectives  | A  | R    | C  | C   | C   | C    | C    | I   |

| Define project constraints | A  | R    | C  | C   | C   | C    | C    | I   |

| Identify required agents   | A  | R    | C  | C   | C   | C    | C    | I   |

| Start project review       | A  | R    | I  | C   | C   | C    | C    | R   |

| Approve project start      | A  | C    | I  | C   | C   | C    | C    | C   |



\---



\# 8. Requirements Engineering RACI



| Activity                         | HO | ORCH | KM | CSE | REQ | COMP | SAFE | AUD |

| -------------------------------- | -- | ---- | -- | --- | --- | ---- | ---- | --- |

| Capture stakeholder needs        | A  | R    | I  | C   | R   | C    | C    | I   |

| Define system requirements       | A  | C    | I  | C   | R   | C    | C    | C   |

| Define regulatory requirements   | A  | C    | I  | C   | C   | R    | C    | C   |

| Define safety requirements       | A  | C    | I  | C   | C   | C    | R    | C   |

| Review requirements completeness | A  | C    | I  | C   | R   | C    | C    | R   |

| Maintain requirements records    | I  | C    | R  | C   | R   | C    | C    | I   |

| Approve requirements baseline    | A  | C    | I  | C   | R   | C    | C    | C   |



\---



\# 9. Architecture RACI



| Activity                        | HO | ORCH | KM | CSE | EE | BMS | ME | SW | COMP | SAFE | AUD |

| ------------------------------- | -- | ---- | -- | --- | -- | --- | -- | -- | ---- | ---- | --- |

| Define system boundaries        | A  | C    | I  | R   | C  | C   | C  | C  | C    | C    | C   |

| Define system architecture      | A  | C    | I  | R   | C  | C   | C  | C  | C    | C    | C   |

| Define electrical architecture  | A  | C    | I  | C   | R  | C   | C  | C  | C    | C    | C   |

| Define battery architecture     | A  | C    | I  | C   | C  | R   | C  | C  | C    | C    | C   |

| Define mechanical architecture  | A  | C    | I  | C   | C  | C   | R  | C  | C    | C    | C   |

| Define software architecture    | A  | C    | I  | C   | C  | C   | C  | R  | C    | C    | C   |

| Review architecture consistency | A  | C    | I  | C   | C  | C   | C  | C  | C    | C    | R   |

| Approve architecture baseline   | A  | C    | I  | R   | C  | C   | C  | C  | C    | C    | C   |

| Document architecture decision  | I  | C    | R  | R   | C  | C   | C  | C  | C    | C    | I   |



\---



\# 10. Make-or-Buy RACI



| Activity                       | HO | ORCH | KM | CSE | EE | BMS | ME | SW | COST | SUP | COMP | SAFE | AUD |

| ------------------------------ | -- | ---- | -- | --- | -- | --- | -- | -- | ---- | --- | ---- | ---- | --- |

| Identify make-or-buy candidate | A  | R    | I  | C   | C  | C   | C  | C  | C    | C   | I    | I    | I   |

| Define evaluation criteria     | A  | C    | I  | R   | C  | C   | C  | C  | C    | C   | C    | C    | C   |

| Technical evaluation           | I  | C    | I  | C   | R  | R   | R  | R  | I    | C   | C    | C    | I   |

| Cost evaluation                | I  | C    | I  | C   | C  | C   | C  | C  | R    | C   | I    | I    | I   |

| Supplier evaluation            | I  | C    | I  | C   | C  | C   | C  | C  | C    | R   | C    | I    | I   |

| Compliance evaluation          | I  | C    | I  | C   | C  | C   | C  | C  | I    | C   | R    | C    | I   |

| Safety evaluation              | I  | C    | I  | C   | C  | C   | C  | C  | I    | I   | C    | R    | I   |

| Consolidate recommendation     | A  | R    | I  | R   | C  | C   | C  | C  | C    | C   | C    | C    | I   |

| Independent review             | I  | C    | I  | C   | C  | C   | C  | C  | C    | C   | C    | C    | R   |

| Approve make-or-buy decision   | A  | C    | I  | C   | C  | C   | C  | C  | C    | C   | C    | C    | C   |

| Document ADR                   | I  | C    | R  | C   | C  | C   | C  | C  | C    | C   | C    | C    | I   |



\---



\# 11. Safety and Compliance RACI



| Activity                             | HO | ORCH | KM | CSE | COMP | SAFE | TEST | AUD |

| ------------------------------------ | -- | ---- | -- | --- | ---- | ---- | ---- | --- |

| Identify applicable regulations      | A  | C    | I  | C   | R    | C    | C    | C   |

| Identify safety-critical functions   | A  | C    | I  | C   | C    | R    | C    | C   |

| Define safety concept                | A  | C    | I  | C   | C    | R    | C    | C   |

| Define compliance strategy           | A  | C    | I  | C   | R    | C    | C    | C   |

| Define required evidence             | A  | C    | I  | C   | R    | R    | C    | C   |

| Review safety argument               | A  | C    | I  | C   | C    | C    | C    | R   |

| Review compliance assumptions        | A  | C    | I  | C   | C    | C    | C    | R   |

| Approve safety-relevant direction    | A  | C    | I  | C   | C    | C    | C    | C   |

| Document safety/compliance decisions | I  | C    | R  | C   | C    | C    | C    | I   |



\---



\# 12. Verification and Validation RACI



| Activity                     | HO | ORCH | KM | CSE | REQ | EE  | BMS | ME  | SW  | TEST | AUD |

| ---------------------------- | -- | ---- | -- | --- | --- | --- | --- | --- | --- | ---- | --- |

| Define verification strategy | A  | C    | I  | C   | C   | C   | C   | C   | C   | R    | C   |

| Define validation strategy   | A  | C    | I  | C   | C   | C   | C   | C   | C   | R    | C   |

| Create test plan             | A  | C    | I  | C   | C   | C   | C   | C   | C   | R    | C   |

| Create test cases            | I  | C    | I  | C   | C   | C   | C   | C   | C   | R    | C   |

| Map requirements to tests    | A  | C    | R  | C   | R   | C   | C   | C   | C   | R    | C   |

| Execute tests                | I  | C    | I  | I   | I   | R/C | R/C | R/C | R/C | R    | I   |

| Review test coverage         | A  | C    | I  | C   | C   | C   | C   | C   | C   | C    | R   |

| Approve test readiness       | A  | C    | I  | C   | C   | C   | C   | C   | C   | R    | C   |

| Document test results        | I  | C    | R  | I   | I   | C   | C   | C   | C   | R    | I   |



\---



\# 13. Documentation and Knowledge RACI



| Activity                            | HO | ORCH | KM | CSE | AUD |

| ----------------------------------- | -- | ---- | -- | --- | --- |

| Maintain repository structure       | A  | C    | R  | I   | I   |

| Maintain documentation index        | I  | C    | R  | I   | I   |

| Maintain ADRs                       | I  | C    | R  | C   | I   |

| Maintain requirements documentation | I  | C    | R  | C   | I   |

| Maintain risk documentation         | I  | C    | R  | C   | I   |

| Maintain review reports             | I  | C    | R  | I   | R   |

| Maintain lessons learned            | I  | C    | R  | I   | C   |

| Maintain changelog                  | I  | C    | R  | I   | I   |

| Publish to Wiki if required         | I  | C    | R  | I   | I   |

| Check documentation completeness    | A  | C    | R  | C   | C   |



\---



\# 14. Tooling RACI



| Activity                      | HO | ORCH | KM | TOOL | AUD |

| ----------------------------- | -- | ---- | -- | ---- | --- |

| Define tool requirements      | A  | R    | C  | C    | I   |

| Configure repository tools    | A  | C    | C  | R    | I   |

| Configure OpenClaw runtime    | A  | C    | C  | R    | I   |

| Configure Telegram interface  | A  | C    | C  | R    | I   |

| Define tool permissions       | A  | C    | C  | R    | C   |

| Review tool governance impact | A  | C    | C  | C    | R   |

| Document tool configuration   | I  | C    | R  | R    | I   |

| Approve tool access change    | A  | C    | I  | R    | C   |



\---



\# 15. Escalation RACI



| Escalation Type                 | Responsible | Accountable | Consulted                      | Informed |

| ------------------------------- | ----------- | ----------- | ------------------------------ | -------- |

| Constitutional conflict         | CG          | HO          | ORCH, AUD                      | KM       |

| Agent role conflict             | ORCH        | HO          | CG, KM                         | AUD      |

| Technical architecture conflict | CSE         | HO          | Specialists, AUD               | KM       |

| Safety concern                  | SAFE        | HO          | CSE, AUD                       | ORCH, KM |

| Compliance uncertainty          | COMP        | HO          | AUD, external expert if needed | ORCH, KM |

| Documentation gap               | KM          | ORCH        | Artifact owner                 | HO       |

| Tooling failure                 | TOOL        | HO          | ORCH, KM                       | AUD      |

| Missing requirement             | REQ         | CSE         | ORCH, Specialists              | KM       |

| Missing verification evidence   | TEST        | CSE         | REQ, AUD                       | KM       |

| Final unresolved issue          | ORCH        | HO          | Relevant agents                | KM       |



\---



\# 16. Initial Responsibility Summary



For the initial EOS setup, the following responsibility model applies:



| Area                  | Primary Responsible                       | Final Accountable |

| --------------------- | ----------------------------------------- | ----------------- |

| Constitution          | Constitution Guardian / Knowledge Manager | Human Owner       |

| AI Organization       | Orchestrator / Knowledge Manager          | Human Owner       |

| Agent Registry        | Knowledge Manager                         | Human Owner       |

| RACI Matrix           | Orchestrator / Knowledge Manager          | Human Owner       |

| Agent Specifications  | Knowledge Manager                         | Human Owner       |

| System Prompts        | Knowledge Manager                         | Human Owner       |

| Workflows             | Orchestrator                              | Human Owner       |

| Repository Structure  | Knowledge Manager                         | Human Owner       |

| OpenClaw Runtime      | Tooling Agent / Human Maintainer          | Human Owner       |

| First Product Project | Chief Systems Engineer / Orchestrator     | Human Owner       |



\---



\# 17. Open Items



The following items remain open:



\* define detailed RACI for each specialist agent,

\* define risk-based approval thresholds,

\* define low-risk fast-track workflow,

\* define branch protection responsibilities,

\* define pull request review ownership,

\* define OpenClaw runtime responsibility model,

\* define Wiki publishing responsibilities,

\* define external expert involvement criteria,

\* define project-specific RACI extension template.



\---



\# 18. Change History



| Version | Date | Change                    | Author   |

| ------- | ---- | ------------------------- | -------- |

| 0.1     | TBD  | Initial RACI Matrix draft | EOS Team |



