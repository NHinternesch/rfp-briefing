---
name: rfp-briefing
description: "Review all RFP documents in a folder and subfolders and draft a concise 1-page summary briefing with the key points from the RFP documents. Use this skill whenever the user asks to review an RFP, summarize an RFP, create an RFP briefing, or asks to review/analyze vendor or procurement documents. Also trigger when the user wants to prepare for an RFP response or understand what an RFP is asking for."
allowed-tools: Read, Bash, Write
effort: medium
tags: [rfp, briefing, summary, procurement, pre-sales]
---

# RFP Briefing

This skill scans all RFP documents in a directory and generates a concise 1-page briefing summarizing the key points.

## Directory Context

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

### Step 1 - Scan all documents
  - Scan all file types, including but not limited to .pdf, .doc, .docx, .xls, .xlsx, .csv, .txt, .ppt, .pptx, etc.

### Step 2 - Extract key information
While scanning, extract:
  - Company/organization details
  - Project scope and requirements
  - Timeline and milestones
  - Budget information
  - Evaluation criteria
  - Submission requirements
  - Key stakeholders and contacts
  - Technical specifications
  - Compliance requirements

### Step 3 — Generate the Briefing

Produce a **1-page briefing** using the RFP Briefing Structure below. Be concise — do not exceed one page.

Save outputs to the project folder:
1. As a `.md` file
2. As a `.docx` Word document — minimal but elegant design, font: **Helvetica**, **grayscale only**


## RFP Briefing Structure

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

## Output Notes

- The briefing must strictly fit on one page — prioritize the most critical information.
- For the Word document, read the docx SKILL.md at before generating, to ensure correct formatting and tooling.
- If key information is missing or ambiguous in the source documents, note it with `[Not specified]` rather than omitting the field.