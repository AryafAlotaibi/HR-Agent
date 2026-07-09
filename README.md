# HR-Agent - Multi-Agent Resume Screening System

## Overview

HR-Agent is a multi-agent AI system that helps HR teams analyze resumes and select suitable candidates based on job requirements.

The system reads candidate resumes, compares skills with the required job skills, calculates a matching score, and provides a final decision.

---

## Agents

### 1. Planner Agent

* Validates candidate data.
* Checks missing inputs.
* Detects prompt injection attempts.

### 2. Resume Analyzer Agent

* Analyzes resume content.
* Matches candidate skills with HR requirements.
* Calculates candidate score.

### 3. Reviewer Agent

* Reviews the score.
* Accepts or rejects candidates based on the decision rule.

---

## Workflow

```
HR Requirements
       |
       v
Planner Agent
       |
       v
Resume Analyzer Agent
       |
       v
Reviewer Agent
       |
       v
Candidate Decision
```

---

## Features

* Multi-agent workflow.
* Resume skill matching.
* Top candidate ranking.
* JSONL file processing.
* Execution logging.
* Security checks:

  * Input validation.
  * Prompt injection detection.

---

## Dataset

The system uses a JSONL file containing candidate resume information:

* Job title
* Skills
* Experience
* Resume text
---


## Project Structure

```
HR-Agent/
│
├── HR.ipynb
├── candidates.jsonl
└── README.md
```
