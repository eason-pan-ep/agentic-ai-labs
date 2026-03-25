# Agentic AI Labs

[![DeepLearning.AI](https://img.shields.io/badge/DeepLearning.AI-Course-0056D2.svg)](https://www.deeplearning.ai/)
[![Claude Code](https://img.shields.io/badge/Claude-Code-191919.svg)](https://claude.ai/code)
[![Python](https://img.shields.io/badge/Python-3.12+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-412991.svg)](https://openai.com/)
[![Gemini](https://img.shields.io/badge/Google-Gemini-4285F4.svg)](https://ai.google.dev/)

Hands-on labs from an Agentic AI course from Deeplearning.AI exploring multi-agent workflows, LLM-based automation, and iterative AI systems.

## Overview

This repository contains practical exercises demonstrating key agentic AI patterns and techniques. Each lab is implemented as an interactive Jupyter notebook with supporting utilities.

## Labs

### Lab 1: Chart Generation with Reflection
An agentic workflow that generates data visualizations through iterative refinement:
- **Generate**: LLM creates matplotlib code from natural language
- **Execute**: Run the generated code to produce a chart
- **Reflect**: LLM analyzes the chart image and critiques the output
- **Refine**: LLM generates improved code based on visual feedback

**Key Concepts**: Code generation, vision models, reflection loops

### Lab 2: SQL Generation with Reflection
An agentic workflow that improves SQL query generation through iterative refinement and external feedback:
- **Generate**: LLM creates SQL queries from natural language questions
- **Execute**: Run the query against an event-sourced transactions database
- **Reflect**: LLM evaluates whether the query results answer the original question
- **Refine**: LLM generates improved SQL based on actual query output feedback

**Key Concepts**: Text-to-SQL, reflection with external feedback, query refinement, event-sourced data modeling

### Lab 3: Turning Functions into Tools
Demonstrates function calling and tool use with LLMs using the Google Gemini API:
- **Function Declaration**: Convert Python functions into LLM-callable tools with automatic or manual schema definition
- **Automatic Tool Calling**: Gemini SDK handles function execution and response integration automatically
- **Multi-Tool Workflows**: Chain multiple tool calls in a single conversation turn
- **Practical Tools**: Weather lookup, file writing, QR code generation with embedded images

**Key Concepts**: Function calling, tool use, automatic function execution, multi-tool orchestration

### Lab 4: Component-Level Evaluation
Demonstrates how to add component-level evaluation to agentic workflows to ensure quality and reliability:
- **Research Pipeline**: Multi-tool research agent using arXiv, Tavily web search, and Wikipedia
- **Domain-Based Evaluation**: Automated quality checks that verify research sources against trusted domain lists
- **Component Testing**: Evaluate individual agent outputs (e.g., checking if search results come from reputable sources)
- **Evaluation Metrics**: Pass/fail checks with detailed reports showing URL extraction, domain matching, and approval ratios

**Key Concepts**: Component-level evaluation, quality assurance, trusted domain validation, research workflows

### Lab 5: Customer Service Agent (Planning in Code)
A customer service agent for a sunglasses store that uses "planning in code" — the LLM writes TinyDB Python as its plan, which is then executed in a controlled sandbox:
- **Plan as Code**: LLM generates executable TinyDB queries wrapped in `<execute_python>` tags instead of calling predefined tools
- **Sandbox Execution**: Generated code runs in a restricted namespace with DB table objects and helper functions injected
- **Multi-Item Transactions**: One transaction row per item; stock validated before any mutation
- **Structured Responses**: Executed code must set `answer_text` (customer-facing reply) and `STATUS` (`success`, `no_match`, `insufficient_stock`, `invalid_request`, `unsupported_intent`)

**Key Concepts**: Planning in code, sandboxed code execution, TinyDB, dynamic query generation, structured LLM output contracts
