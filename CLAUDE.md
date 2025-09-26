# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

jedrasiak:scientia is an Integrated Knowledge Management Environment (IKME) designed to store and manage knowledge as a graph structure. The project follows a monorepo structure with apps and packages directories.

## Architecture

The environment consists of 5 main applications:
1. **cli** - Command line interface for managing databases with single line terminal commands
2. **tui** - Text-based user interface
3. **desktop** - Electron app built with vanilla JS, CSS, HTML, WebComponents, and SQLite
4. **server** - Cloud database server that desktop clients can connect to
5. **web** - Web interface for working with cloud databases via browser

## Project Structure

- `apps/` - Main applications (currently empty, awaiting implementation)
- `packages/` - Shared packages and libraries (currently empty, awaiting implementation)
- `specs/` - Project specifications and documentation
  - `specs/overview.md` - Main project overview and terminology

## Key Terminology

- **scrinium** - A local folder which contains database file and media folder

## Development Status

This appears to be a new project in the initial setup phase. The apps and packages directories are currently empty, indicating the project structure is prepared but implementation hasn't begun yet.