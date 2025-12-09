# Markup AI - Microsoft Power Automate Custom Connector

## Introduction

The Markup AI Custom Connector for Microsoft Power Automate enables seamless integration of advanced document processing and AI-powered markup capabilities into your automated workflows. With this connector, you can leverage Markup AI's intelligent document analysis, annotation, and extraction features directly within Power Automate flows.

This custom connector empowers users to:
- Automate document processing workflows with AI-driven markup and annotation
- Integrate document analysis capabilities into business process automation
- Streamline document-heavy workflows with automated markup and validation

## Folder Structure

### `/src`
Contains all raw source files for the Power Automate connector, including:
- YAML configuration files defining the connector's structure and operations
- Images and icons used in the connector interface
- Core connector definitions and metadata

### `/src/solutions`
Contains pre-built solutions, helpers, and sample workflows that can be downloaded and used directly in Power Automate. These solutions demonstrate best practices and common use cases for the Markup AI connector.

### `/package`
Contains all files required for custom connector submission to Microsoft AppSource, including:
- Package manifest and configuration
- Compliance and certification materials
- Deployment assets and documentation

### `/docs`
Contains general documentation, guides, and helper resources:
- Integration guides and tutorials
- Recipes and usage examples
- Technical specifications

## Quick Start

Get started quickly with these ready-to-use guides:

- **[Automated Content Monitoring with Power Automate for SharePoint and Teams](./docs/receipes.md)** - Quick Start guide showing how to create a content monitoring workflow in SharePoint and Teams using the Markup AI connector

## Content Monitoring Helper Solution

The **Markup AI Content Monitoring Tools** solution is available as an unmanaged solution at `/src/solutions/MarkupAIContentMonitoringTools_1_0_0_0.zip`. This helper solution provides two reusable child flows that simplify common document analysis tasks:

#### 1. Markup AI - Generate Document Analysis Report HTML
Generates a comprehensive document analysis report in your preferred format:
- **HTML format** - Perfect for embedding in email notifications with styled content
- **Adaptive Card format** - Optimized for posting rich, interactive messages to Microsoft Teams

**Required Parameter:**
- `Markup AI Workflow ID` - The unique identifier of the Markup AI workflow to generate the report for

#### 2. Markup AI - Wait for Check Result
**Note: Use this flow only if the webhook pattern can't be used!**

Provides intelligent polling functionality to wait for document check completion:
- Automatically polls the Markup AI service for check results
- Continues the parent flow execution once the check result is available
- Handles asynchronous document processing seamlessly


These helper flows can be imported into your Power Automate environment and called as child flows from your own automation workflows, significantly reducing development time for common content monitoring scenarios.

## Getting Started

Refer to the documentation in the `/docs` folder for detailed setup instructions and usage examples.

## License

See [LICENSE](LICENSE) for more information.
