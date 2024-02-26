<div align="center">

![devchat](https://github.com/devchat-ai/devchat/assets/592493/f39979fe-fe32-410b-bf9d-2118ac8ea3d5)

# DevChat: Intelligent Scripts that Streamline Your Dev Workflows

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![CircleCI](https://circleci.com/gh/devchat-ai/devchat/tree/main.svg?style=shield)](https://circleci.com/gh/devchat-ai/devchat/tree/main)
[![GitHub license](https://img.shields.io/github/license/devchat-ai/devchat.svg)](https://github.com/devchat-ai/devchat/blob/main/LICENSE)
[![Downloads](https://pepy.tech/badge/devchat)](https://pepy.tech/project/devchat)
[![PyPI version](https://badge.fury.io/py/devchat.svg)](https://badge.fury.io/py/devchat)
[![Discord Chat](https://img.shields.io/discord/1106908489114206309?logo=discord)](https://discord.gg/9t3yrbBUXD)

**Harness AI-Powered Scripts in Your IDE with a Dynamic Chat GUI**

🧩 Develop AI-powered scripts in a unified framework with minmized efforts to handle IDEs and LLMs.

🛠️ Tailor the AI coding assistant to align perfectly with your specific needs.

✨ Elevate your text chats with a dynamic, Markdown-rendered GUI for enhanced interaction.

</div>

## What is DevChat?

DevChat is an open-source workflow engine that enables developers to craft scripts for:
- Engaging with users through a chat panel within their IDEs, facilitating the completion of development tasks.
- Creating intelligent, automated workflows for these tasks, utilizing the full potential of various large language models (LLMs).

DevChat combines the flexibility of script writing, the cutting-edge capabilities of latest AI models, and an enriched user experience through intuitive chat GUI.

## Why DevChat?

While numerous AI coding tools exist, many still struggle to adeptly handle nuanced scenarios inherent in bespoke development processes. For instance, your team might adhere to a specific coding format that existing products don't support configuration for. Or, you desire an automated workflow to run tests and, upon encountering an error, allow AI to attempt a fix, but only once to avoid likely subsequent failures. Such specific functionalities are often not fully realized in available products.

At its core, we believe that the creativity and productivity of developers are yet to be fully unleashed. Our aim with DevChat is to simplify the integration of AI in software development to the level of writing a script, thereby unlocking new possibilities for developers.

## Core Features

### IDE Chat Panels

- [Visual Studio Code extension](https://github.com/devchat-ai/devchat-vscode) from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat).

- [IntelliJ Platform plugin](https://github.com/devchat-ai/devchat-intellij) from [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/23258-devchat).

### ChatMark

Documentation: https://docs.devchat.ai/chatmark-markdown-spec.

### IDE Services

### Mannual Context Building

Great output requires great input. To maximize the power of AI, DevChat assists you to mannually select **the optimal context** to the AI.

- For instance, to generate test cases for a function, you can add an existing test case. The test case serves as a useful reference for DevChat, enabling it to understand how to write a valid test case specific to your environment, thus eliminating the need for you to specify every requirement in your prompt.

  ![Add to context](https://github.com/devchat-ai/devchat-vscode/assets/592493/9b19c798-d06f-4373-8f8a-6a950c3a8ba5)

- You can incorporate the output of any command, such as `tree ./src`, into a prompt with DevChat. For example, you can add the output of `git diff --cached` to DevChat, which can then generate a commit message for you.

  ![Generate a commit message](https://github.com/devchat-ai/devchat-vscode/assets/592493/7bd34547-762c-4f97-b792-8d05a9eb1dcf)

- Program analysis can assist in building the necessary context. Suppose you want DevChat to explain some code to you. DevChat can perform better if it's aware of the dependent functions that the code is calling. In this scenario, you can select the target code with DevChat to explain and add "symbol definitions" to the context (by clicking the plus button). DevChat will then generate a prompt that explains the target code, taking into account the dependent functions.

## Workflow Examples

- Automatically rename poorly-named local variables for improved readability: [/refactor.names](https://github.com/devchat-ai/workflows/tree/main/refactor/names).
- Generate unit tests of a function: [/unit_tests](https://github.com/devchat-ai/workflows/tree/main/unit_tests).

## Quick Start

For GUI, install our [IDE extension or plugin](https://docs.devchat.ai/quick-start/installation).

For CLI:
- Install Python 3.8+ and [pip](https://pip.pypa.io/en/stable/installation/).
- Install DevChat by running: `pip install devchat`.
- Set your [OpenAI API Key](https://platform.openai.com/account/api-keys) by running `export OPENAI_API_KEY="[sk-...]"` (or DevChat access key).
- To access help, use the command: `devchat --help` or `devchat prompt --help`.

## Contributing

- Repositories:
  - The core library and CLI: https://github.com/devchat-ai/devchat
  - System default workflows: https://github.com/devchat-ai/workflows
  - Visual Studio Code extension: https://github.com/devchat-ai/devchat-vscode
  - IntelliJ Platform plugin: https://github.com/devchat-ai/devchat-intellij

- Issues and pull request are welcome: https://github.com/devchat-ai/devchat/issues

- Join our [Discord](https://discord.gg/9t3yrbBUXD)!

## What is Prompt-Centric Software Development (PCSD)?

- The traditional code-centric paradigm is evolving. Stay ahead of the curve with DevChat.

- Write prompts to create code. Transform prompts into all the artifacts in software engineering.

  <img width="600" alt="image" src="https://github.com/devchat-ai/devchat/assets/592493/dd32e900-92fd-4fa4-8489-96ed17ab5e0e">

  <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
  
- We like to call it DevPromptOps
  
  <img width="500" alt="image" src="https://github.com/devchat-ai/devchat/assets/592493/e8e1215b-53b0-4473-ab00-0665d33f204a">
  
  <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>

## Contact
  
Email: hello@devchat.ai

We are creators of [Apache DevLake](https://devlake.apache.org/).
