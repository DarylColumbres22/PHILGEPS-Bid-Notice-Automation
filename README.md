# PHILGEPS Bid Notice Abstraction and Extraction Automation

**Project Type:** Internship Project  
**Organization:** Actimai Philippines  
**Automation Platform:** UiPath  
**Framework:** Robotic Enterprise Framework (REFramework)

## Overview

This project involved a UiPath-based automation workflow for extracting bid notice information from the Philippine Government Electronic Procurement System (PHILGEPS) website.

The automation uses browser automation, data extraction, and validation techniques to streamline the collection and processing of bid notice information.

The workflow is built using UiPath's Robotic Enterprise Framework (REFramework), which provides a structured approach to transaction processing, logging, exception handling, and recovery.

## My Contributions

As an intern, I assisted with the automation workflow and related tasks, including:

- Supporting bid notice information extraction from PHILGEPS.
- Working with UiPath-based browser automation processes.
- Assisting with data extraction and validation.
- Supporting information accuracy and consistency checks.

## Automation Framework

The project uses the **UiPath Robotic Enterprise Framework (REFramework)**, built on top of the Transactional Business Process template.

Key framework features include:

- State Machine-based automation structure.
- Logging, exception handling, and recovery.
- Configuration management through `Config.xlsx`.
- Credential management through Orchestrator Assets and Windows Credential Manager.
- Transaction retrieval and status updates.
- Screenshots captured during system exceptions.

## Input and Output Files

### Input File

`Data/Input/Input.xlsx`

- Contains the reference IDs to be processed.
- Records with a `Success` status are skipped and will not be processed again.

### Output File

`Data/Output/Output.xlsx`

- Stores the results of processed transactions.
- Every transaction is appended to the output file.

## Workflow Process

The automation follows four major phases:

1. **Initialize Process**
   - Loads configuration settings.
   - Retrieves application credentials.
   - Opens and logs in to the required applications.

2. **Get Transaction Data**
   - Retrieves transactions from the configured Orchestrator Queue or another configured data source.

3. **Process Transaction**
   - Executes the transaction-specific workflow.
   - Updates transaction status as Success, Business Rule Exception, or System Exception.

4. **End Process**
   - Logs out and closes the applications used during execution.

## Technologies and Concepts

- UiPath Studio
- Robotic Enterprise Framework (REFramework)
- RPA (Robotic Process Automation)
- Browser Automation
- Data Extraction
- Excel Data Processing
- Data Validation
- Exception Handling
- Transaction Processing

## Project Scope

This was completed as part of my internship at Actimai Philippines. My involvement focused on assisting with the automation workflow and related extraction and validation tasks.

The framework structure and core REFramework implementation were based on the automation engineer's existing project.

## Documentation

Additional project documentation is included in the `Documentation` folder.

## Security Notes

Sensitive credentials, private data, and proprietary implementation details are excluded from this repository.

