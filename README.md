# Autogen_Multi_Agent_Pattern_With_Code_Execution

This project utilizes Autogen, an AI conversational agent framework, to facilitate multi-agent discussions and code execution. The workflow includes several advisors with defined roles, enabling collaboration through nested chats.

## Advisors and Roles

The system supports multiple advisors, each with specific roles:
- **Flow of Advisors:** Advisors engage in structured discussions to provide insights and recommendations.
- **Code Execution Capability:** Each advisor can execute code, such as web scraping for information, simulations, and data analysis, to support their recommendations.
  - *Note:* Ensure to set `use_docker=True` in code execution configuration for enhanced security.

## Workflow Overview

The system operates through nested chats managed by Autogen’s GroupChatManager, facilitating advisor discussions based on predefined messages. The workflow includes:

1. **Initialization:** Advisors initiate discussions based on a predefined initial message to formulate comprehensive plans.
   
2. **Advisor Inputs:** Advisors provide insights through multi-round discussions facilitated by Autogen, ensuring diverse perspectives are integrated into the final plan.
   
3. **Customizability:** Advisors and initial messages can be customized to fit specific domains or scenarios.

## Example Use Case

The following example demonstrates how to initiate discussions and integrate advisor inputs:

```python
# Python code snippet demonstrating agent initialization and conversation initiation
import autogen
from autogen import ConversableAgent, GroupChat, GroupChatManager

# Example configuration using Autogen and API key
llm_config = {"model": "gpt-4o", "api_key": "your_api_key_here"}

# Detailed Python code snippet example provided previously
