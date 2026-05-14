# Architecture

## High-Level Architecture

FlowScope AI is a lightweight, documentation-first MVP assembled through no-code and AI tooling rather than a traditional monolithic codebase.

## Main Components

### 1. Landing Layer

- Built with Lovable
- Explains the product value
- Provides product positioning
- Sends users to the Telegram bot

### 2. Interaction Layer

- Telegram bot as the main user interface
- Receives raw business requests
- Supports a natural-language input flow

### 3. Automation Layer

- n8n orchestrates the workflow
- Handles routing logic and process transitions
- Connects input, AI processing, and output generation

### 4. AI Core

- OpenAI API used for request understanding and structured reasoning
- Supports clarification logic
- Supports task classification
- Supports scenario routing and response generation

### 5. Data / Artifact Layer

- Google Sheets for storing or managing structured workflow data
- Google Docs for report generation and supporting artifacts

## MVP Workflow Logic

Raw request -> clarification -> classification -> routing -> selected workflow -> structured result

## Why This Architecture Fits the Hackathon

- fast to assemble
- easy to demo
- easy to evolve
- well suited for a Telegram-first product
- enough flexibility to support multiple future workflows

## Future Architecture Growth

Potential next additions:

- workflow library for multiple SMB scenarios
- lightweight admin dashboard
- analytics around request categories and completion
- memory / history for repeated business users
- modular prompt and routing configuration
