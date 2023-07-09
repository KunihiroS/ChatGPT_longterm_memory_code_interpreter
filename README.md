# ChatGPT Long-Term Memory Emulation with Log.json

This project involves a system that uses a `log.json` file to emulate a form of long-term memory for ChatGPT, OpenAI's language model. 

The `log.json` file contains two sections: `metadata` and `entries`. 

- `metadata`: Contains details about when the file was created and last updated, who created the file, and the version of the file format.
- `entries`: A list of entries that log past dialogues or knowledge. Each entry is a dictionary with at least these keys: `type`, `content`, and `timestamp`.

The system interacts with the `log.json` file in two main use cases:

- **Use Case 1 - Creation of a New Log File**: If a `log.json` file does not already exist, the system will create a new one. 

- **Use Case 2 - Updating an Existing Log File**: If a `log.json` file is provided, the system reads the file, and then updates the file after each conversation step.

This system pays close attention to the way it logs the conversation into the 'entries' section, carefully analyzing the conversation content to categorize it correctly.

This project is a step towards making ChatGPT more context-aware and providing it with a mechanism to refer back to past dialogues or knowledge. This can be particularly useful in ongoing, long-term conversations where context and memory are important.

Please refer to specification files for more detailed information.
