## Primary Objective

The main objective of Claude Code when working in this directory is to review all RFP documents in this folder and subfolders and draft a concise 1-page summary briefing with the key points from the RFP documents. 

## Directory Overview

This directory contains RFP (Request for Proposal) documents of a buyer looking to purchase an enterprise SaaS solution. 
The documents consist of various file types, such as Word documents, PDFs, Excel sheets, Power Point presentations, etc.

## Vendor Expert Groups

The following expert groups are available to contribute to the RFP submission:

- **Solutions Engineering**: Subject matter experts (SMEs) for product features, technical requirements, functional requirements, technical specifications, roadmap items, and tool integrations
- **Security & Privacy**: SMEs for data protection, security measures, compliance, and privacy regulations
- **Legal**: SMEs for contractual and legal topics
- **Architecture**: SMEs for technical architecture, infrastructure, scalability, performance, and system integrations
- **Services & Strategy**: SMEs for implementation services, professional services, consulting, deployment, service level agreements, maintenance, and ongoing assistance
- **Sales Director**: Main RFP coordinator and SME for pricing, commercial terms, contract negotiations, business value propositions, sales-related inquiries, and high-level company strategy and positioning
- **Executive Sponsor & SVP**: Responsible for executive support, sign-off, and business relationship

Additional expert groups may be added in the future as needed.

## Workflow

When tasked to create an RFP briefing, the workflow consists of:

1. **Scan all documents** 
  - Scan all file types, including but not limited to .pdf, .doc, .docx, .xls, .xlsx, .csv, .txt, .ppt, .pptx, etc.
  - To process Excel files, convert them to readable format using the Bash tool with Python. If the needed packages are not available, the agent will attempt to install them automatically.

2. **Extract key information** including:
  - Company/organization details
  - Project scope and requirements
  - Timeline and milestones
  - Budget information
  - Evaluation criteria
  - Submission requirements
  - Key stakeholders and contacts
  - Technical specifications
  - Compliance requirements

3. **Generate a 1-page briefing** 
  - Strictly adhere to the structure outlined in the section RFP Briefing Content below
  - Ensure conciseness, output should not exceed one page
  - Save the briefing as an .md file to the project folder
  - Also save the briefing as a .doc Word document to the project folder. Use a minimal but elegant design, use the font Helvetica and only use grayscale font color.

## RFP Briefing Content

When generating the briefing, make sure to adhere to the 1 page format.
The briefing should follow this structure:

**RFP Overview**
- **Client:** [Organization name]
- **Project Context:** [Brief description]
- **High-Level Business Objectives:** [2-3 key objectives]
- **Value:** [Budget/contract value]
- **Contract Terms:** [Expected contract terms]
- **Timelines:** [List all important dates, e.g. issue date, Q&A date, submission date, presentation date, decision date etc.]

**Key Requirements**
- [Top 3-5 most critical requirements]

**SLA Requirements**
- [List SLA requirements and associated penalties]

**Evaluation Criteria**
- [Scoring methodology and weights]

**Incumbent & Competitive Landscape**
- [Insights on incumbent, currently used solution to be replaced]
- [Insights on competitors]

**Risks & Challenges**
- [Potential challenges or red flags]
- [Non-negotiable requirements that could be impossible for the vendor to meet]

**Submission Requirements**
- [List the required information and documents to be supplied by the vendor]

**Required Content Contributiors**
- [Identify the vendor expert groups that are needed to contribute content (see details about vendor expert groups below). If possible, indicate the estimated amount of input required from each expert group on a 3-step scale: Low, medium, high]