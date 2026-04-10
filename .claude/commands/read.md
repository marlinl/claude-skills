---
description: Onboard the agent into the MarlinL Engineering Skillset and initialize specific module contexts.
---

## Phase 1: Context Inventory
1. **Locate Root Metadata**: Search for the root `SKILL.md` and `marketplace.json` to understand the overall architecture.
2. **Identify Tech Stack**: Verify if the current environment aligns with:
   - Java 21/25 (check for Virtual Threads, Scoped Values, or Sealed Classes).
   - Spring Boot 4.0.x (check `pom.xml` or `build.gradle` for dependency versions).
   - Domain-Driven Design (DDD) or Clean Architecture indicators.

## Phase 2: Skill Module Analysis
If a specific folder is provided (e.g., `/read spring-boot-patterns`), perform a deep dive:
1. **Read `SKILL.md`**: Parse the specific module's rules, patterns, and constraints.
2. **Load Patterns**: If the folder contains `.java` templates or `rules.json`, index them as primary coding standards.
3. **Verify Compliance**: Scan the existing codebase against the "Rules" section of the selected skill.

## Phase 3: Executive Summary
Output a concise "Engineering Snapshot" to the user:
- **Active Skill**: [Module Name]
- **Target Architecture**: [e.g., Spring Boot 4 / Hexagonal]
- **Constraints Loaded**: List the top 3 high-priority rules (e.g., "Enforce Constructor Injection," "Mandatory @Tag for Tests").
- **Next Step Recommendation**: Suggest a specific refactoring or audit task based on the loaded skill.

## Rules for Claude
- Do NOT ignore the `POWERFUL Tier` designation; provide high-level architectural advice, not just syntax fixes.
- If the project is in a transition state (e.g., migrating from Spring Boot 3.5 to 4.0), prioritize identifying deprecated API usage.

