# Project README

## Overview
This project is built to simulate an agent that uses language models to achieve predefined goals by interacting with its environment through various actions. The primary goals of the agent are to gather information from project files and terminate its session by providing the content of its findings in a specified format.

## Components\n\n

### 1. Agent 
The `Agent` class is the core component of this project. It orchestrates the interaction between goals, agent language, actions, and environment. It constructs prompts based on its memory and goals, generates responses using the language model, executes actions, and updates itself based on the results.

### 2. Agent Language
Defined in `agent_language.py`, this component facilitates the communication by constructing prompts and interpreting responses specifically formatted for use with LLMs.

### 3. Environment
The `Environment` class in `environment.py` is responsible for executing actions as defined by the agent and handles any errors that might occur during execution.

### 4. Goals and Actions
Goals are the objectives that the agent aims to achieve, while actions are tasks the agent can perform to achieve these goals. The `goals_actions.py` file defines classes for creating and managing goals and actions within an action registry.

### 5. LLM Call
Using the `llm_call.py` module, the agent interacts with a language model to generate responses from prompts that it constructs during its run cycle.

### 6. Memory
`Memory` is used to keep track of past interactions and maintain a coherent state over time. It allows for pruning irrelevant or large parts of memory to avoid context overflow.

### 7. Main Execution
The `main.py` serves as the entry point of the application, setting up parameters and initiating the agent's run sequence based on user input and goals.

## Usage
    - The agent is designed to read each file ending with `.py` in its directory, process the content, and ultimately output a structured summary to the user.
    - Use the `main.py` file to execute the example run provided in the repository.\n\n## Installation\nThis project requires Python and the `litellm` library for completion engine calls. Ensure that all dependencies are covered by using Python package managers or manual installation via provided requirements.
---
The current design integrates memory and action-based interactions, adaptive prompts for adjusted retries, and structured results for seamless process flows as initiated by main goals set within the agent's architecture.\nTerminating...", 'timestamp': '2025-03-21T17:05:49+0530'
