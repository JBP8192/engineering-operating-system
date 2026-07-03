\# Prompts



This directory contains executable prompt implementations for agents in the Engineering Operating System.



Agent specifications are stored in:



`../500\_agent\_specifications/`



Prompts are implementations of those specifications.



A prompt shall not be treated as the agent definition itself.  

The agent definition is the specification.  

The prompt is the current executable version.



\## Structure



\- `system/core/` – core EOS agents

\- `system/specialists/` – specialist agents

\- `tests/` – prompt test conversations and expected behavior



\## Rules



1\. Every active prompt must reference an agent specification.

2\. Every active prompt must have a version.

3\. Every active prompt must have a change history.

4\. Every active prompt must be tested before activation.

5\. Prompt changes must be documented.

