# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Microsoft 365 MCP (Model Context Protocol) server project designed to provide unified access to Microsoft Graph API services. The project is currently in the specification phase, containing comprehensive OpenAPI definitions for Microsoft 365 services but no implementation code yet.

## Architecture

### API Specifications Structure
- **Location**: `/specs/` directory contains 40+ OpenAPI 3.0.4 specification files
- **Organization**: Specs are organized by Microsoft 365 service areas:
  - **Identity & Access**: Applications.yml, Identity.DirectoryManagement.yml, Identity.Governance.yml, Users.yml
  - **Communication**: Mail.yml, Calendar.yml, Teams.yml, CloudCommunications.yml
  - **Collaboration**: Files.yml, Sites.yml, Groups.yml, Notes.yml
  - **Device Management**: DeviceManagement.yml and related files
  - **Security & Compliance**: Security.yml, Compliance.yml
  - **Business Apps**: Planner.yml, Bookings.yml, Education.yml
- **API Base**: All specs target `https://graph.microsoft.com/v1.0/`
- **Reference**: Full Microsoft Graph OpenAPI spec available at https://github.com/microsoftgraph/msgraph-metadata/blob/master/openapi/v1.0/openapi.yaml

### Current State
- No implementation code exists yet
- No build system or package configuration files present
- Project is in planning/specification gathering phase
- Technology stack for implementation not yet determined

## Development Notes

### When Implementation Begins
- Choose appropriate MCP server framework/language
- Establish build system and development commands
- Update this file with specific build, test, and development commands
- Consider code generation from OpenAPI specs for consistent API surface

### API Coverage
The specifications provide comprehensive coverage of Microsoft Graph v1.0 including:
- User and group management
- Mail, calendar, and contacts
- File storage and SharePoint
- Teams and communication
- Device and application management
- Security and compliance features
- Business application integrations