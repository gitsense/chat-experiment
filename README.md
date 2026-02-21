<!--
Component: GitSense Chat README
Block-UUID: d5df0235-c5c8-4ae7-8a99-02ae710d54ca
Parent-UUID: 84313538-6e88-4652-a8b8-ec7295a91592
Version: 1.6.0
Description: A comprehensive README for GitSense Chat, detailing its purpose, features, licensing, and initial installation.
Language: Markdown
Created-at: 2025-08-16T18:39:38.050Z
Authors: Gemini 2.5 Flash Thinking (v1.0.0), Gemini 2.5 Flash Thinking (v1.1.0), Gemini 2.5 Flash Thinking (v1.2.0), Gemini 2.5 Flash Thinking (v1.3.0), Gemini 2.5 Flash Thinking (v1.4.0), GPT OSS 120B (v1.5.0), GPT OSS 120B (v1.6.0)
-->


> [!IMPORTANT]
> **This repository has been renamed from `chat` to `chat-experiment` and is no longer maintained.**
> The official GitSense Chat repository is now located at: **[https://github.com/gitsense/chat](https://github.com/gitsense/chat)**

# GitSense Chat

GitSense Chat is reimagining how we can interact with Large Language Models (LLMs) to build better software, together. It provides an effective, intuitive environment for building highly relevant context, generating traceable code, managing knowledge, creating custom AI search assistants and more.

**🚀 Try GitSense Chat Live: [https://chat.gitsense.com](https://chat.gitsense.com)**

![GitSense Chat Home Page Screenshot](https://github.com/gitsense/chat/raw/main/assets/images/gitsense-chat-home-page-bordered.png)

## Table of Contents

*   [Why Use GitSense Chat?](#why-use-gitsense-chat)
    *   [No Lock-in, Just Better Workflows](#no-lock-in)
    *   [Your Personal AI Search Assistant](#your-personal-ai-search-assistant)
    *   [Context Engineering](#context-engineering)
    *   [Next-Gen Knowledge Base](#next-gen-knowledge-base)
    *   [And More](#and-more)
*   [License and Business Model](#license-and-business-model)
    *   [License](#license)
    *   [Business Model](#business-model)
*   [Installation](#installation)
    *   [NPM](#npm)
    *   [Docker](#docker)
*   [Post-Installation Configuration & Usage](#post-installation-configuration--usage)
    *   [Quick Start](#quick-start)

<a id=why-use-gitsense-chat></a>
## Why Use GitSense Chat?
GitSense Chat is more than just a chat interface; it's a powerful platform designed to transform how users interact with their information and AI. Here are some of its key features:

<a id=no-lock-in></a>
### No Lock-in, Just Better Workflows

GitSense Chat is designed to be your **starting point for every LLM conversation**, not a walled garden. We empower you to define precise context, generate traceable code, and manage knowledge with great efficiency. Once you've crafted your perfect LLM interaction, our **Messages Tool** makes it dead simple to extract and copy your conversation content-including code, notes, and context-for seamless use in your IDE, other LLM solutions, or any documentation.

We're confident that once you experience the clarity, control, and traceability GitSense Chat provides, you'll want to come back for its other rich features. Our goal is to enhance your existing workflows, not replace them.

![No Lock-in](https://github.com/gitsense/chat/raw/main/assets/images/no-lock-in-bordered.png)

<a id=your-personal-ai-search-assistant></a>
### Your Personal AI Search Assistant

Simply chat with an LLM to make your data smarter. With GitSense Chat, you can turn any text-based data into intelligent insights that can help you find bugs faster, identify security vulnerabilities, and even organize your grocery bills. For example, you could ask, "find all files with high-priority TODOs in the `mobile-app-ios` and `mobile-app-android` repositories," and have AI search your GitSense Chat knowledge base to find answers that traditional text searches like grep can't.

![Personal AI Search Assistant Screenshot](https://github.com/gitsense/chat/raw/main/assets/images/personal-ai-search-assistant-bordered.png)

<a id=context-engineering></a>
### Context Engineering

Significantly improve the accuracy, relevance, and cost-efficiency of LLM responses by precisely managing the context you provide. GitSense Chat provides intuitive tools to build, refine, and manage the LLM's knowledge base, ensuring it always has the most relevant data for any task.

![Context Engineering](https://github.com/gitsense/chat/raw/main/assets/images/context-engineering-bordered.png)

<a id=next-gen-knowledge-base></a>
### Next-Gen Knowledge Base

Create a wiki that you can truly chat with, offering a dynamic and conversational experience unlike traditional wikis. This transforms how technical documents and training materials are created and consumed, fostering a more interactive and accessible learning environment.

![Knowledge Base](https://github.com/gitsense/chat/raw/main/assets/images/knowledge-base-bordered.png)

<a id=and-more></a>
### And More

Explore GitSense Chat's full potential by loading your own personal help guide directly within the application. Visit [https://chat.gitsense.com](https://chat.gitsense.com) to chat with the documentation, ask questions, and learn interactively about all features, from advanced context management to custom AI tools.

<a id=license-and-business-model></a>
## License and Business Model

GitSense Chat is provided under a **Fair License**, permitting internal, non-commercial use and modification. Copying for profit or redistribution, or use in directly competing products/services, is strictly prohibited without explicit permission.

Our business model focuses on ensuring the long-term sustainability and continued development of the platform through a commercial version of the **GitSense Chat Bridge**.

[Read the full license details below.](#full-license-details)  
[Learn more about our business model below.](#full-business-model-details)

<a id=installation></a>
## Installation

This section covers the initial steps to get GitSense Chat up and running. For detailed configuration, starting/stopping the application, and using the administration tool, please refer to the [Post-Installation Configuration & Usage Guide](#post-installation-configuration--usage).

<a id=npm></a>
### NPM

Run GitSense Chat directly using Node.js and npm.

#### Prerequisites

*   [Node.js](https://nodejs.org/) (version 20 or higher recommended) and npm installed.
*   [Git](https://git-scm.com/downloads) for cloning the repository.

#### 1. Clone the Repository

```bash
git clone https://github.com/gitsense/chat.git
cd chat

```

#### 2. Install Dependencies

```bash
npm install
```

#### 3. Initial Environment Variables Setup

```bash
cp .env.example .env
```

<a id=docker></a>
### Docker

Run GitSense Chat as a Docker container for easy setup and portability.

#### Prerequisites

*   [Docker Desktop](https://www.docker.com/products/docker-desktop/) (Windows/macOS) or [Docker Engine](https://docs.docker.com/engine/install/) (Linux).

#### 1. Download the Docker Image

```bash
docker pull gitsense/chat
```

#### 2. Retrieve Helper Tools and Configuration

```bash
mkdir -p ~/gitsense-chat-docker
cd ~/gitsense-chat-docker

curl -o gsc-docker https://raw.githubusercontent.com/gitsense/chat/main/bin/gsc-docker
curl -o .env.example https://raw.githubusercontent.com/gitsense/chat/main/.env.example
chmod +x gsc-docker
```

#### 3. Initial Environment Variables Setup

```bash
cp .env.example .env
```

<a id="post-installation-configuration--usage"></a>
## Post-Installation Configuration & Usage

<a id="quick-start"></a>
### Quick Start

#### Default Models (pre-configured)

GitSense Chat ships with four ready-to-use LLM models:

| Model                | Provider   | Model ID                     | Default? |
|----------------------|------------|------------------------------|----------|
| **Claude 4.0 Sonnet** | Anthropic  | `claude-sonnet-4-20250514`  | - |
| **Gemini 2.5 Pro**    | Google     | `gemini-2.5-pro`            | - |
| **GPT-5**             | OpenAI     | `gpt-5`                     | - |
| **GPT OSS 120B**      | OpenRouter | `openai/gpt-oss-120b`       | - |

> To set default model, please refer to **[docs/POST_INSTALLATION.md](docs/POST_INSTALLATION.md)** for more information.

#### Required API Keys

Add the following keys to your `.env` file (or the Docker-mounted `.env`):

```dotenv
# Anthropic (Claude)
ANTHROPIC_API_KEY="sk-YOUR_ANTHROPIC_KEY"

# Google Gemini
GEMINI_API_KEY="YOUR_GEMINI_KEY"

# OpenAI (GPT-5)
OPENAI_API_KEY="sk-YOUR_OPENAI_KEY"

# OpenRouter (GPT OSS 120B)
OPENROUTER_API_KEY="YOUR_OPENROUTER_KEY"
```

> **Tip:** Only the keys for the providers you plan to use are required. 

#### Starting GitSense Chat

```bash
# NPM installation
npm start
```

```bash
# Docker installation
gsc-docker start
```

Both commands launch the server at **http://localhost:3357**.

#### Need More Help?

Once the server is up, launch the Help Guide by clicking the **Load Personal Help Guide** link, located below the chat input field. The built-in LLM assistant can walk you through:

* Adding or removing models via `gsc-admin`
* Configuring additional providers
* Advanced usage tips and troubleshooting

Feel free to ask the assistant any follow-up questions-it's there to make your onboarding as smooth as possible.

For detailed instructions on all post-installation tasks, please refer to the dedicated guide. In that guide you'll learn how to:

* **Configure your API keys** for every supported provider (OpenAI, Anthropic, Google Gemini, OpenRouter, etc.).
* **Add, remove, or reorder models** - including how to create new custom models or delete the defaults.
* **Create visual dividers** in the model list to keep your configuration tidy.
* **Restore a previous `chat.json` backup** if you ever need to roll back changes.
* **Start and stop the application** for both NPM-based and Docker-based installations, with commands for checking status and viewing logs.
* **Use the `gsc-admin` CLI** to manage providers, models, and configuration without editing JSON manually.
* **Enable and customize the help guide** inside GitSense Chat, so you can chat with an LLM for on-the-fly assistance.
* **Understand the versioning and author history** embedded in each configuration block.

You can find the full guide here: **[docs/POST_INSTALLATION.md](docs/POST_INSTALLATION.md)**

---

<a id=full-license-details></a>
## Full License Details 

The JavaScript files in this repository are currently provided in a minified distribution. While we finalize the adoption of the **Fair License**, the core terms are as follows:

You are permitted to use and modify this software for **internal, non-commercial purposes**. This means you can integrate GitSense Chat into your workflows, adapt it to your specific needs, and learn from its codebase. However, **copying for profit or redistribution is strictly not permitted**, nor can this software be used to develop or enhance any product or service that directly or indirectly competes with GitSense Chat without explicit permission. Once the Fair License is formally adopted, the unminified source code will be made freely available under these terms.

<a id=full-business-model-details></a>
## Full Business Model Details

GitSense Chat is designed to be a free-to-use application, providing **significant** value to individual developers and teams. Our business model focuses on ensuring the long-term sustainability and continued development of the platform through a commercial offering of the **GitSense Chat Bridge**.

GitSense Chat's **key strength** lies in its ability to import and manage software development data, such as Git repositories, and coordinate indexing at scale. The free version of the GitSense Chat Bridge, while functional, has inherent limitations due to its JavaScript implementation, which currently lacks support for multithreading and other advanced performance optimization capabilities.

Our goal is to generate revenue by charging for a commercial version of the GitSense Chat Bridge. This commercial bridge will offer enhanced performance and scalability, along with significantly more powerful search features, allowing companies to create advanced context engines for use when chatting with LLMs. This approach enables us to keep the core GitSense Chat application free and accessible to everyone, fostering a wide user base while monetizing the specialized, high-performance data ingestion component that is critical for enterprise-level adoption.
