\# Communication Model



\*\*Document ID:\*\* 200-004

\*\*Title:\*\* Communication Model

\*\*Version:\*\* 0.1 Draft

\*\*Status:\*\* Proposed

\*\*Owner:\*\* Engineering OS Orchestrator

\*\*Parent Document:\*\* `200\_organization/AI\_ORGANIZATION.md`

\*\*Related Documents:\*\*



\* `000\_constitution/EOSC\_v0.1.md`

\* `200\_organization/AGENT\_REGISTRY.md`

\* `200\_organization/RACI\_MATRIX.md`



\*\*Applies to:\*\* All human-agent, agent-agent and tool-agent communication within the Engineering Operating System.



\---



\# 1. Purpose



This document defines how communication flows inside the Engineering Operating System.



It describes:



\* how the human owner interacts with the EOS,

\* how requests are routed,

\* how agents communicate,

\* how results are consolidated,

\* how reviews are requested,

\* how documentation updates are triggered,

\* how escalation works,

\* how tool-based communication is controlled.



The purpose of this document is to prevent uncontrolled, inconsistent or undocumented communication between agents.



The EOS shall communicate like an engineering organization, not like a loose collection of chatbots.



\---



\# 2. Core Communication Principle



The Engineering OS Orchestrator is the primary communication hub.



The human owner should normally communicate with the EOS through the Orchestrator, not directly with every specialist agent.



The Orchestrator receives the request, determines the required work, routes tasks to relevant agents, consolidates the results and returns a coherent response.



Specialist agents contribute expertise.



The Auditor reviews.



The Knowledge Manager documents.



The Human Owner decides.



\---



\# 3. Default Communication Flow



The default flow is:



```text

Human Owner

&#x20;   ↓

User Interface

&#x20;   ↓

Engineering OS Orchestrator

&#x20;   ↓

Specialist Agents

&#x20;   ↓

Engineering OS Orchestrator

&#x20;   ↓

Independent Auditor if required

&#x20;   ↓

Engineering OS Orchestrator

&#x20;   ↓

Human Owner

&#x20;   ↓

Engineering Knowledge Manager

&#x20;   ↓

Repository / Wiki / Knowledge Base

```



This flow may be simplified for low-risk tasks.



It shall not be bypassed for:



\* safety-relevant decisions,

\* regulatory questions,

\* architecture decisions,

\* agent governance changes,

\* prompt changes,

\* tool permission changes,

\* project baseline changes,

\* make-or-buy decisions.



\---



\# 4. Communication Layers



The EOS uses five communication layers.



\## 4.1 Human Interface Layer



This is the interface between the human owner and the EOS.



Possible interfaces:



\* Telegram

\* OpenClaw chat interface

\* GitHub issues

\* Pull requests

\* Confluence or Wiki comments

\* direct local development environment



Primary purpose:



\* receive human intent,

\* return consolidated answers,

\* ask for human decisions,

\* communicate risks and open questions.



\## 4.2 Orchestration Layer



This layer is owned by the Engineering OS Orchestrator.



Primary purpose:



\* understand intent,

\* classify the request,

\* identify required agents,

\* create work packages,

\* coordinate specialist responses,

\* consolidate results,

\* request reviews,

\* trigger documentation.



\## 4.3 Specialist Layer



This layer consists of domain agents.



Primary purpose:



\* provide expert input,

\* identify assumptions,

\* identify risks,

\* create domain-specific recommendations,

\* define required evidence,

\* identify dependencies to other domains.



\## 4.4 Assurance Layer



This layer consists of review and audit agents.



Primary purpose:



\* independently review outputs,

\* identify findings,

\* classify risks,

\* verify traceability,

\* recommend approval, conditional approval or rejection.



\## 4.5 Knowledge Layer



This layer is owned by the Engineering Knowledge Manager.



Primary purpose:



\* document decisions,

\* maintain ADRs,

\* update requirements,

\* update risks,

\* maintain lessons learned,

\* maintain agent registry,

\* maintain prompt and workflow documentation.



\---



\# 5. Communication Roles



\## 5.1 Human Owner



The Human Owner defines intent, priorities and final decisions.



The Human Owner may request work, approve decisions, reject recommendations or ask for clarification.



The Human Owner is the final accountable party for product, project and organizational decisions.



\## 5.2 Engineering OS Orchestrator



The Orchestrator is the communication coordinator.



The Orchestrator shall not silently perform all work itself when specialist agents are required.



The Orchestrator shall:



\* classify the request,

\* select relevant agents,

\* define expected outputs,

\* consolidate responses,

\* identify contradictions,

\* communicate open questions,

\* request review when needed,

\* request documentation updates.



\## 5.3 Specialist Agents



Specialist agents communicate domain-specific input.



Specialist agents shall not directly approve final decisions.



Every specialist response should include:



\* assumptions,

\* analysis,

\* recommendation,

\* risks,

\* dependencies,

\* required evidence,

\* confidence level.



\## 5.4 Independent Auditor



The Auditor communicates findings.



The Auditor does not become the designer of the solution under review.



Audit outputs shall include:



\* review scope,

\* findings,

\* severity,

\* evidence gaps,

\* required rework,

\* approval recommendation.



\## 5.5 Engineering Knowledge Manager



The Knowledge Manager communicates documentation status.



The Knowledge Manager shall identify when a decision, requirement, risk, review result or lesson learned must be written to the repository or Wiki.



The Knowledge Manager shall not own the technical decision itself.



\---



\# 6. Request Classification



Every incoming request shall be classified before execution.



| Class | Description                   | Example                             | Review Required |

| ----- | ----------------------------- | ----------------------------------- | --------------- |

| C0    | Simple information request    | “Where is this file?”               | No              |

| C1    | Low-risk documentation task   | “Add this to README.”               | Usually no      |

| C2    | Engineering analysis          | “Compare two motor options.”        | Maybe           |

| C3    | Architecture decision         | “Choose 48 V or 72 V.”              | Yes             |

| C4    | Safety or compliance relevant | “Is this brake concept sufficient?” | Yes             |

| C5    | Governance or agent change    | “Create a new agent.”               | Yes             |

| C6    | Constitution change           | “Modify EOS principles.”            | Mandatory       |



The Orchestrator performs the initial classification.



If classification is uncertain, the request shall be treated as the higher-risk class.



\---



\# 7. Routing Rules



\## 7.1 Default Routing



| Request Type          | Primary Agent                   | Supporting Agents                          |

| --------------------- | ------------------------------- | ------------------------------------------ |

| General coordination  | Orchestrator                    | Knowledge Manager                          |

| Constitution question | Constitution Guardian           | Orchestrator                               |

| Agent organization    | Orchestrator                    | Knowledge Manager, Constitution Guardian   |

| Agent registry update | Knowledge Manager               | Orchestrator                               |

| Prompt change         | Knowledge Manager               | Constitution Guardian, Orchestrator        |

| System architecture   | Chief Systems Engineer          | Specialist Agents, Auditor                 |

| Requirements          | Requirements Engineer           | Chief Systems Engineer, Compliance, Safety |

| Safety topic          | Functional Safety Agent         | Auditor, Chief Systems Engineer            |

| Compliance topic      | Homologation \& Compliance Agent | Auditor, Chief Systems Engineer            |

| Electrical topic      | Electrical Engineering Agent    | BMS, Software, Safety                      |

| Battery topic         | Battery \& BMS Agent             | Electrical, Safety, Compliance             |

| Mechanical topic      | Mechanical Engineering Agent    | Test, Compliance                           |

| Software topic        | Software / Embedded Agent       | Cybersecurity, Test, Safety                |

| Testing topic         | Test \& Validation Agent         | Requirements, Specialist Agents            |

| Supplier topic        | Supplier Strategy Agent         | Cost, Compliance, Specialist Agents        |

| Cost topic            | Cost Engineering Agent          | Supplier Strategy, Chief Systems Engineer  |

| Documentation topic   | Knowledge Manager               | Artifact Owner                             |

| Tooling topic         | Tooling Agent                   | Orchestrator, Knowledge Manager            |



\---



\# 8. Standard Message Structure



Agent-to-agent communication should follow a structured format.



\## 8.1 Work Package Request



```text

Work Package ID:

Requested by:

Assigned to:

Context:

Objective:

Inputs:

Expected Output:

Constraints:

Deadline / Priority:

Review Required:

Documentation Required:

```



\## 8.2 Specialist Response



```text

Work Package ID:

Agent:

Summary:

Assumptions:

Analysis:

Recommendation:

Risks:

Dependencies:

Required Evidence:

Open Questions:

Confidence:

```



\## 8.3 Auditor Response



```text

Review ID:

Reviewed Artifact:

Review Scope:

Result:

Findings:

\- Blocker:

\- Major:

\- Minor:

\- Observations:

Required Rework:

Approval Recommendation:

```



\## 8.4 Documentation Request



```text

Documentation Request ID:

Source:

Artifact Type:

Decision / Requirement / Risk / Lesson:

Summary:

Owner:

Target Location:

Required Links:

Status:

```



\---



\# 9. Consolidation Rules



The Orchestrator consolidates specialist contributions into one coherent response.



The consolidated response shall:



\* remove duplication,

\* preserve important disagreements,

\* identify assumptions,

\* identify open questions,

\* identify risks,

\* separate facts from recommendations,

\* identify required decisions,

\* identify required documentation updates.



The Orchestrator shall not hide disagreement between agents.



If agents disagree, the disagreement shall be explicitly stated and escalated if necessary.



\---



\# 10. Review Communication



A review shall be requested when:



\* the topic affects architecture,

\* safety is affected,

\* compliance is affected,

\* evidence is missing,

\* an agent acts outside its scope,

\* requirements are unclear,

\* a decision has high cost impact,

\* a workflow or prompt changes governance behavior.



The Auditor shall receive:



\* artifact under review,

\* review scope,

\* relevant assumptions,

\* linked requirements,

\* linked decisions,

\* known risks.



The Auditor shall return:



\* finding list,

\* severity classification,

\* required rework,

\* recommendation.



The Auditor may not silently correct and approve the same artifact.



\---



\# 11. Documentation Triggers



The Knowledge Manager shall be triggered when any of the following occurs:



\* new requirement,

\* changed requirement,

\* new architecture decision,

\* changed architecture decision,

\* new risk,

\* changed risk,

\* new agent,

\* changed agent,

\* prompt change,

\* workflow change,

\* tool configuration change,

\* review result,

\* project milestone,

\* lesson learned,

\* unresolved open issue.



Undocumented decisions are considered unstable.



\---



\# 12. Tool Communication



Tools are communication channels and execution environments.



Tools are not decision makers.



\## 12.1 Telegram



Telegram is a human interface.



It may be used for:



\* quick user requests,

\* status questions,

\* task routing,

\* notifications,

\* summaries.



Telegram shall not be the source of truth for decisions.



Important decisions from Telegram must be transferred into the repository or Wiki.



\## 12.2 OpenClaw



OpenClaw is the runtime environment for agents and workflows.



It may coordinate:



\* agent execution,

\* tool calls,

\* memory access,

\* workflow automation,

\* Telegram interaction.



OpenClaw shall follow the governance rules defined in this repository.



\## 12.3 GitHub



GitHub is the source of truth for versioned artifacts.



It stores:



\* Constitution,

\* governance documents,

\* organization documents,

\* agent specifications,

\* prompts,

\* workflows,

\* templates,

\* ADRs,

\* project documentation,

\* schemas,

\* changelogs.



GitHub is preferred for anything that must be versioned.



\## 12.4 Wiki / Confluence



The Wiki explains the organization and project knowledge in human-friendly form.



It may contain:



\* onboarding pages,

\* process explanations,

\* architecture overviews,

\* decision summaries,

\* lessons learned,

\* project dashboards.



The Wiki may reference GitHub artifacts but should not replace version-controlled source documents.



\## 12.5 Local Files



Local files may be used during drafting.



Important local files must eventually be committed to GitHub or explicitly marked as temporary.



\---



\# 13. Source of Truth Rules



Every information type shall have a defined source of truth.



| Information Type           | Source of Truth                         |

| -------------------------- | --------------------------------------- |

| Constitution               | GitHub                                  |

| Governance documents       | GitHub                                  |

| Agent registry             | GitHub                                  |

| Agent specifications       | GitHub                                  |

| Prompts                    | GitHub                                  |

| Workflows                  | GitHub                                  |

| ADRs                       | GitHub                                  |

| Requirements               | GitHub or dedicated requirements system |

| Risks                      | GitHub or dedicated risk register       |

| Review reports             | GitHub                                  |

| Wiki explanations          | Wiki / Confluence                       |

| Temporary chat discussions | Telegram / OpenClaw                     |

| Final decisions            | GitHub ADR or approved document         |

| Lessons learned            | GitHub and optionally Wiki              |



If information exists in multiple places, the defined source of truth prevails.



\---



\# 14. Escalation Communication



Escalation shall happen when:



\* an agent cannot complete a task,

\* required input is missing,

\* two agents disagree,

\* safety or compliance is affected,

\* evidence is insufficient,

\* scope is unclear,

\* the Constitution may be violated,

\* documentation is missing,

\* tool behavior is unexpected.



Escalation format:



```text

Escalation ID:

Raised by:

Issue:

Affected Artifact:

Severity:

Reason:

Required Decision:

Recommended Escalation Target:

Deadline / Urgency:

```



\---



\# 15. Communication with the Human Owner



The EOS shall communicate with the Human Owner in a concise but transparent way.



Human-facing responses should include:



\* what was understood,

\* what was done,

\* what is recommended,

\* what remains open,

\* what requires human decision.



For high-risk topics, the EOS shall explicitly state:



\* assumptions,

\* limitations,

\* required expert review,

\* safety or compliance uncertainty.



The EOS shall not present uncertain conclusions as final certainty.



\---



\# 16. Fast-Track Communication



Low-risk tasks may use a simplified flow.



Examples:



\* add a README section,

\* create a placeholder document,

\* summarize an existing document,

\* format a Markdown file,

\* add a non-critical template.



Fast-track flow:



```text

Human Owner

&#x20;   ↓

Orchestrator

&#x20;   ↓

Knowledge Manager or relevant agent

&#x20;   ↓

Repository update

```



Fast-track shall not be used for:



\* safety,

\* compliance,

\* architecture baseline,

\* agent activation,

\* Constitution changes,

\* supplier commitments,

\* final product decisions.



\---



\# 17. Communication Anti-Patterns



The following patterns are prohibited:



1\. Specialist agents making final decisions without review.

2\. Auditors designing and approving the same solution.

3\. Telegram being treated as permanent documentation.

4\. Important decisions remaining only in chat history.

5\. Multiple conflicting sources of truth.

6\. Agents modifying prompts without documentation.

7\. Tool automation bypassing human approval.

8\. Requirements being created after implementation decisions.

9\. Agent-to-agent disagreement being hidden from the human owner.

10\. Safety or compliance uncertainty being presented as resolved.



\---



\# 18. Initial Runtime Model



For the initial EOS implementation, the expected communication path is:



```text

Human Owner

&#x20;   ↓

Telegram or OpenClaw UI

&#x20;   ↓

Engineering OS Orchestrator

&#x20;   ↓

Selected Agents

&#x20;   ↓

Independent Auditor if needed

&#x20;   ↓

Engineering Knowledge Manager

&#x20;   ↓

GitHub Repository

&#x20;   ↓

Wiki / Confluence if needed

```



The first runtime implementation may be manual.



Automation shall be introduced only after the communication model is stable.



\---



\# 19. Open Items



The following items remain open:



\* define exact Telegram command structure,

\* define OpenClaw agent routing implementation,

\* define message schema for work packages,

\* define where prompts are stored,

\* define when Wiki publishing is required,

\* define notification rules,

\* define escalation severity levels,

\* define review request template,

\* define documentation request template,

\* define agent-to-agent memory rules,

\* define GitHub issue usage rules,

\* define pull request communication rules.



\---



\# 20. Change History



| Version | Date | Change                            | Author   |

| ------- | ---- | --------------------------------- | -------- |

| 0.1     | TBD  | Initial communication model draft | EOS Team |



