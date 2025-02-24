# SWE Development Kit (SWEKit.js)

Build and benchmark Software Engineering agents with Composio's tooling ecosystem using JavaScript

## Overview

SWE Development Kit (swekit) is a powerful framework for building Software Engineering agents using Composio's tooling ecosystem. 
It provides tools like Github, Repo Indexing, Repo Search, File Manager, Shell Manager, and more.

## Key Features

- **Agent Scaffolding**: Quickly create Devin like agents that work out-of-the-box with popular agentic frameworks like OpenAI, Langchain, and more.
- **Flexible Workspace Environments**: Operate your agents within a variety of secure and isolated environments including Docker, E2B, and FlyIO for security and isolation.
- **Customizable Tools**: Add or optimize your agent's abilities with a variety of tools.
- **Benchmarking**: Evaluate your agents against the SWE-bench, a comprehensive benchmark for software engineering tasks.

## Getting Started

### Installation

Begin by installing the core packages using your favourite package manager. The recommended method is using `pnpm`, but you can also use `npm` or `yarn`.

```bash
pnpm install -g composio-core
```

### Required API Keys

Create a `.env` file in the root directory of your project and add the following API keys:

```env
E2B_API_KEY=<your_e2b_api_key>
OPENAI_API_KEY=<your_openai_api_key>
COMPOSIO_API_KEY=<your_composio_api_key>
```

To obtain these API keys:
- E2B API Key: Sign up at [e2b.dev](https://e2b.dev)
- OpenAI API Key: Get from [OpenAI Platform](https://platform.openai.com)
- Composio API Key: Available at [Composio Dashboard](https://app.composio.dev)

### Connect GitHub Integration

You have two options to set up the GitHub integration:

#### Option 1: Using CLI
Run the following command with your Composio API key:
```bash
COMPOSIO_API_KEY=<composio_access_token> composio-js add github
```

#### Option 2: Using Web Interface
1. Visit [Composio Dashboard](https://app.composio.dev)
2. Navigate to Integrations
3. Enable and configure the GitHub integration

### Clone SWE Template for JS

> **Warning**: To use Docker as the default workspace environment, ensure your Docker server is running.

To quickly get started, clone the template from GitHub using the command below:
```bash
git clone https://github.com/ComposioHQ/swe-js-template.git swe-js
```

### Install all the dependencies

Install all the required dependencies for the SWE agent using `pnpm`, which is the recommended package manager:
```bash
cd swe-js && pnpm i
```

### Run your SWE agent

To start the agent, just run the following command:
```bash
pnpm start
```
You will be prompted to specify the repository and issue for the agent to address.

