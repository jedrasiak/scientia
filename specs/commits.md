# Conventional Commits Cheatsheet

This document outlines the conventional commit standards for jedrasiak:scientia project.

## Format

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

## Types

- **feat**: New feature for the user
- **fix**: Bug fix for the user
- **docs**: Changes to documentation
- **style**: Formatting, missing semicolons, etc; no production code change
- **refactor**: Refactoring production code, eg. renaming a variable
- **test**: Adding missing tests, refactoring tests; no production code change
- **chore**: Updating grunt tasks etc; no production code change

## Scopes

Project-specific scopes for jedrasiak:scientia:

- **cli**: Command line interface
- **tui**: Text-based user interface
- **desktop**: Electron desktop application
- **server**: Cloud database server
- **web**: Web interface
- **core**: Core functionality shared across apps
- **db**: Database operations and schema
- **graph**: Graph data structure operations
- **scrinium**: Local folder/database management
- **specs**: Project specifications and documentation

## Examples

### Features
```
feat(cli): add command to create new scrinium
feat(desktop): implement knowledge graph visualization
feat(server): add user authentication system
feat(db): support for graph node relationships
```

### Bug Fixes
```
fix(tui): resolve navigation issue in main menu
fix(desktop): correct SQLite connection handling
fix(graph): fix infinite loop in node traversal
fix(cli): handle missing scrinium directory gracefully
```

### Documentation
```
docs(specs): update project architecture overview
docs(desktop): add WebComponents usage guide
docs: update installation instructions
```

### Refactoring
```
refactor(core): extract common graph operations
refactor(desktop): simplify component lifecycle management
refactor(db): optimize query performance
```

### Tests
```
test(cli): add unit tests for scrinium commands
test(graph): add integration tests for node operations
test(server): add authentication middleware tests
```

### Chores
```
chore: update project dependencies
chore(desktop): configure Electron build pipeline
chore(specs): organize documentation structure
```

## Breaking Changes

For breaking changes, add `!` after the type/scope:

```
feat(cli)!: change scrinium command syntax
refactor(core)!: restructure graph API interface
```

Or add `BREAKING CHANGE:` in the footer:

```
feat(desktop): add new graph visualization engine

BREAKING CHANGE: previous visualization API is no longer supported
```

## Guidelines

1. Use lowercase for type and scope
2. Keep description under 50 characters
3. Use imperative mood ("add" not "added" or "adds")
4. Don't end description with a period
5. Reference issues/PRs in the body when applicable
6. Use scope to indicate which app/component is affected
7. Do not include AI-generated attribution or mentions of AI tools in commit messages