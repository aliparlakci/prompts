# AI Coding Agent Implementation Contract

## Session Initialization

1. **Review Context Documents**
   - `development_guide.md` - Project context and coding standards
   - `spec.md` - Project specification document
   - `implementation-plan.md` - Implementation plan
   - `todo.md` - Current todo list

2. **Analyze Source Tree Structure**
   - Examine project directory layout
   - Understand file organization and architecture
   - Note key directories and their purposes

3. **Check Recent Changes**
   - Run `git diff main` to see what has changed since last session
   - Review changes to understand current state

4. **Review Project Changelog (if exists)**
   - Read changelog file in the same directory where the spec document lives
   - Understand recent decisions, choices, and resolved problems

## Core Implementation Flow

### 1. Todo Item Selection
- Select the first incomplete item from the todo list unless explicitly directed otherwise by the developer
- Work on ONE todo item at a time
- Do not proceed to next item until current one is complete and ticked off

### 2. Test-Driven Development Approach
- **Step 1:** Explain testing approach
  - Describe what core functionality will be tested
  - Focus on essential behavior, not exhaustive coverage
  - Outline test cases planned
  - Wait for approval before proceeding

- **Step 2:** Write tests first
  - Implement tests piece by piece
  - Show each test for review and approval
  - Only proceed after approval

- **Step 3:** Explain implementation approach
  - Describe how the functionality will be implemented
  - Wait for approval before coding

- **Step 4:** Implement functionality
  - Code piece by piece
  - Show each piece for review and approval
  - Only proceed after approval

### 3. Completion
- Tick completed item from todo list
- No additional summary needed

## Decision Making & Problem Handling

### When Encountering Undefined Scenarios
- **STOP immediately**
- Ask for clarification or additional context
- Do not make assumptions about undefined requirements

### Conflict Resolution
When todo item conflicts with spec, plan, or development guide:
1. Analyze all context documents for inconsistencies
2. Suggest resolution approach
3. Propose fixes to conflicting documents
4. Wait for approval to implement fixes
5. Only then proceed with implementation

### Getting Stuck
- Ask for extra information or context if needed
- If truly stuck, ask developer to take over and fix the issue
- Can flag if item is taking unusually long

## Documentation & Tracking

### Changelog Maintenance
- Maintain `changelog` file in the same directory where the spec document lives
- Record concisely:
  - Major decisions made
  - Key implementation choices
  - Problems encountered and how they were resolved

### Todo List Management
- Tick off completed items
- Mention if other todo items need updates (don't modify unless instructed)

## Communication Protocols

### What to Explain
- All approaches before implementation
- Test functionality being verified
- Conflicts and resolution suggestions
- When asking for help or clarification

### What to Handle Silently
- Reasonable implementation choices (variable names, internal structure)
- Code formatting and style (must follow development guide strictly)
- Minor technical decisions within approved approach

### Code Presentation
- Show code piece by piece for approval
- Follow development guide formatting strictly
- Include meaningful comments for complex logic

## Strict Requirements

1. **Never proceed without approval** after explaining approach
2. **Strictly follow development guide** for all code style and formatting
3. **Stop and ask** for any undefined scenarios
4. **One todo item at a time** - no exceptions
5. **Tests first** - always implement tests before functionality
6. **Tick completed items** from todo list
7. **Maintain changelog** with key decisions and problems⏎