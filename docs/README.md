# Architectural Documentation & Profile Overview

This directory (`/docs`) acts as the central source of truth for the architectural decisions and best practices I follow in my projects. Following a robust documentation strategy, I believe every repository should have a standardized documentation structure.

## Overview

### 1. Mindset and Architecture
- **Problem-Driven Development**: Tools like Kubernetes, Docker, Terraform, and various CI/CD solutions are means to an end. The core focus is always the architectural problem: scaling, resilience, security, and developer experience.
- **Distributed Systems**: Handling state, network partitions, and consistency gracefully. It's about what the system provides, the resulting value, and the problems it solves, rather than just adopting the latest hype.
- **Security First (DevSecOps)**: Security shouldn't be an afterthought. It's integrated into the CI/CD pipeline and the initial architectural design.

### 2. Best Practices Followed
- **Clean Code & SOLID**: Prioritizing readability and maintainability.
- **Conventional Commits**: Structuring git commit messages with `feat:`, `fix:`, `chore:`, etc. for automated semantic versioning and changelogs.
- **Documentation First**: Maintaining clear, up-to-date documentation in a `/docs` folder for architectural references (ADRs - Architecture Decision Records) and deployment guides.

### 3. The Automation (GitHub Actions)
This repository contains a GitHub Action (`.github/workflows/snake.yml`) to automatically generate a `github-contribution-grid-snake.svg` which consumes my contribution graph. It runs periodically via cron and pushes the output to the `output` branch, which is then rendered on the main profile README.
