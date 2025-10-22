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
