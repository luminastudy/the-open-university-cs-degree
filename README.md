# Open University of Israel - Computer Science B.Sc. Degree

This repository contains the course structure for the Computer Science Bachelor's degree (B.Sc.) from the Open University of Israel, formatted for the Lumina Study platform.

## Overview

The degree program consists of **120 credits** organized into four main sections:

### א - Mathematics Foundation Studies (35 credits)
Required foundational mathematics courses including:
- Discrete Mathematics
- Linear Algebra 1 & 2
- Calculus 1 & 2
- Probability and Statistics

### ב - Computer Science Studies (At least 70 credits)

#### Required Courses (42-46 credits)
Core computer science courses including:
- Introduction to Computer Science (Java)
- Data Structures and Algorithms
- Operating Systems
- Programming Languages
- Computer Organization
- Logic for Computer Science
- And more...

#### Elective Courses (24-28 credits)
Choose from 29 advanced courses including:
- Artificial Intelligence
- Machine Learning
- Database Systems
- Computer Networks
- Cryptography
- Cyber Security
- Data Mining
- Computer Graphics
- And more...

### ג - Seminar Requirements (6 credits)

#### Seminar Studies (3 credits)
Choose one seminar from 18 options in various CS topics

#### Workshop Studies (3 credits)
Choose one workshop from 11 options for hands-on learning

### ד - General Electives (9 credits)
Free choice from Open University courses

## Degree Requirements

- **Total Credits:** 120
- **Science Credits:** At least 111
- **Computer Science Credits:** At least 76
- **Advanced CS Credits:** At least 27

## Data Structure

The course data is stored in `lumina.json` following the `@lumina-study/block-schema` v0.2 specification **exactly**.

### Schema Compliance

All blocks contain **only** the required schema fields:
- **id** (UUID format): Unique identifier
- **title** (object): Bilingual titles with `he_text` and `en_text`
- **prerequisites** (array): Block dependencies (currently empty, to be added)
- **parents** (array): Parent block references for hierarchical structure

No additional metadata is included to ensure strict schema compliance.

### UUID Format

Block IDs use UUID format:
- Course blocks: Deterministic format based on course codes
  - Format: `{courseCode}000-0000-0000-0000-000000000001`
  - Example: Course 20476 → `20476000-0000-0000-0000-000000000001`
- Section/subsection blocks: Standard UUID v4 format
  - Example: `a1b2c3d4-e5f6-4a7b-8c9d-0e1f2a3b4c5d`

## Repository Structure

```
B.Sc. in Computer Science (root)
├─ A - Mathematics Foundation Studies (6 courses)
├─ B - Computer Science Studies (39 courses)
├─ C - Computer Science Seminar Requirements
│  ├─ I. Seminar Studies in Computer Science (18 courses)
│  └─ II. Workshop Studies in Computer Science (11 courses)
└─ D - General Electives
```

Total: **81 blocks** (1 degree + 6 sections/subsections + 74 courses)

## Current Status

✅ All courses extracted and structured
✅ Schema v0.2 compliant (no extra fields)
🔄 Prerequisites: In progress
  - Linear Algebra 1 → Linear Algebra 2
  - Calculus 1 → Calculus 2
⏳ More prerequisites to be added

## Source

Data extracted from: https://academic.openu.ac.il/cs/computer/program/AF.aspx
(ידיעון תשפ"ו - Academic year 2025-2026)

## License

This data is extracted from publicly available information from the Open University of Israel.
