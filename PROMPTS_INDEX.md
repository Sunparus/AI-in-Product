# PROMPTS_INDEX

## 1. Directory Organization
- **/system**: Contains system-level prompts focused on the overall behavior and rules guiding the agents.
- **/audience**: Houses prompts tailored for specific audience segments based on their needs and interests.
- **/domain**: Focused on domain-specific prompts that provide expertise in certain areas.
- **/feedback**: Includes prompts related to collecting feedback and refining the agents' performance based on user interactions.

## 2. Naming Conventions
- Prompt files are named using the following convention: `agent_<agent_number>_prompt_<description>_v<version_number>.md`
- Each prompt is versioned to track changes and improvements, with the version incrementing according to semantic versioning principles (major.minor.patch).

## 3. Prompt Anatomy
Each prompt follows a standard structure:
- **System Instruction**: Guidelines that dictate how the agent should behave or respond.
- **Context Injection**: Information specific to the task at hand that provides background to the agent.
- **Few-shot Examples**: Example interactions that illustrate expected behavior or responses.
- **Quality Gates**: Criteria that must be met for the prompt to be considered successful.
- **Output Format**: Specification of how the output should be structured and presented.

## 4. Integration Rules
- Agents load prompts at startup by scanning the relevant subdirectory for prompts.
- Prompts must be in an executable format that the agents can interpret correctly.
- The agents utilize the prompts based on their specific requirements and contexts.

## 5. Version Management
- Prompts should be updated based on feedback from AGENT 8 after testing and evaluation of effectiveness.
- Major updates are tracked and communicated to the team to ensure everyone uses the latest versions.

## 6. Monthly Prompt Review Cycle
- A monthly review is conducted to analyze engagement data and QA logs to identify areas for improvement.
- Thresholds for engagement and response accuracy are established to guide revisions.

## 7. Prompt Testing
- New prompts must be validated in a test environment before being rolled out.
- Testing includes checking for correctness, consistency, and adherence to quality gates.

## Agent to Prompt Set Table
| Agent Number | Prompt Set(s) Used |
|--------------|--------------------|
| AGENT 1     | audience, domain   |
| AGENT 2     | system, audience    |
| AGENT 3     | domain, feedback    |
| AGENT 4     | system, feedback    |
| AGENT 5     | audience            |
| AGENT 6     | domain              |
| AGENT 7     | system              |
| AGENT 8     | feedback            |