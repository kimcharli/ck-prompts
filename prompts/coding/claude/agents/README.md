# Claude Sub-Agent Examples for Coding

https://docs.anthropic.com/en/docs/claude-code/sub-agents

This document outlines useful cases for leveraging Claude's sub-agent feature in coding workflows.

## 1. Code Review and Refinement Agent

**Parent Agent Task:** "Review the attached pull request for potential bugs, style violations, and suggest improvements."

**Sub-Agent Functionality:**
- **Linter Agent:** Automatically runs linting tools (e.g., ESLint, Black, Prettier) on the code and reports violations.
- **Security Agent:** Scans for common security vulnerabilities (e.g., SQL injection, XSS) and flags potential risks.
- **Performance Agent:** Analyzes code for performance bottlenecks and suggests optimizations (e.g., algorithmic improvements, caching strategies).
- **Documentation Agent:** Checks for missing or incomplete documentation (e.g., Javadoc, docstrings) and suggests additions.

## 2. Feature Implementation Agent

**Parent Agent Task:** "Implement a user authentication module with sign-up, login, and password reset functionalities."

**Sub-Agent Functionality:**
- **Frontend Agent:** Develops the user interface components (e.g., React, Vue) for authentication forms.
- **Backend Agent:** Implements the API endpoints and business logic for user management (e.g., Node.js, Python/Django).
- **Database Agent:** Designs and creates the necessary database schemas and handles data persistence.
- **Testing Agent:** Writes unit and integration tests for the implemented features to ensure correctness and robustness.

## 3. Bug Fixing and Debugging Agent

**Parent Agent Task:** "Investigate and fix the reported bug in the user profile update functionality."

**Sub-Agent Functionality:**
- **Log Analysis Agent:** Parses application logs to identify error patterns and trace the origin of the bug.
- **Code Tracing Agent:** Steps through the relevant code paths, potentially with dynamic instrumentation, to pinpoint the exact line causing the issue.
- **Test Case Generation Agent:** Creates minimal reproducible test cases that expose the bug.
- **Patch Generation Agent:** Proposes and applies code changes to fix the bug, ensuring existing tests still pass.

## 4. Technology Migration Agent

**Parent Agent Task:** "Migrate the existing monolithic application from Python 2 to Python 3."

**Sub-Agent Functionality:**
- **Syntax Conversion Agent:** Automatically converts Python 2 syntax to Python 3 using tools like `2to3`.
- **Dependency Update Agent:** Identifies and updates incompatible library dependencies to their Python 3 compatible versions.
- **Testing Agent:** Runs existing test suites and identifies new failures due to migration, then assists in fixing them.
- **Code Modernization Agent:** Suggests and applies Python 3 specific idioms and best practices to the converted codebase.
