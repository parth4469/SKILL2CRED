# Skill2Cred --- From Experience to Credential

> **AI-Assisted Recognition of Prior Learning (RPL)**\
> Transforming informal work experience into measurable, NSQF-aligned
> competency evidence and verifiable digital credentials.

## Overview

**Skill2Cred** is an AI-assisted Recognition of Prior Learning (RPL)
platform designed to help workers convert skills gained through informal
work, apprenticeships, and on-the-job experience into structured,
evidence-based competency profiles.

The platform combines:

-   **30% Vernacular Voice Assessment** for knowledge, experience and
    decision-making
-   **70% Practical Skill Assessment** using structured hands-on tasks
-   **AI-assisted competency mapping** against QP/NOS/NSQF requirements
-   **Computer vision** for safety/PPE verification
-   **Standardized scoring rubrics**
-   **Skill-gap identification and targeted remediation**
-   **Human-in-the-loop certification**
-   **W3C Verifiable Credentials with QR verification**
-   **Offline-first assessment with later synchronization**

> **Core principle:** AI assists the assessment; the authorized human
> assessor makes the final competency/certification decision.

## Problem

India has a large informal workforce whose skills are often acquired
through work experience rather than formal education. These workers may
have strong practical competence but lack a reliable way to demonstrate
it through formal certification.

RPL processes can face challenges including:

-   Difficulty documenting informal experience
-   Language and literacy barriers
-   Inconsistent practical assessment
-   Limited assessment infrastructure
-   Assessor workload and variation
-   Connectivity limitations
-   Difficulty verifying evidence
-   Weak linkage between certification and employment

Skill2Cred addresses these gaps through an **AI-assisted, evidence-first
and assessor-led RPL workflow**.

## Solution

``` text
Experience
    ↓
Vernacular Knowledge Assessment
    ↓
Practical Skill Demonstration
    ↓
Evidence Collection + AI Assistance
    ↓
QP / NOS / NSQF Competency Mapping
    ↓
Competency Score + Skill Gap
    ↓
Targeted Skill Bridge (if required)
    ↓
Retest
    ↓
Human Assessor Approval
    ↓
Verifiable Digital Credential
```

## Assessment Model

  -----------------------------------------------------------------------------
  Component                                   Weight Purpose
  --------------------- ---------------------------- --------------------------
  Vernacular Viva                                30% Knowledge, experience and
                                                     decision-making

  Practical Assessment                           70% Demonstrated hands-on
                                                     competence

  AI Assistance                        Support layer Evidence, scoring
                                                     assistance and competency
                                                     mapping

  Human Assessment                   Final authority Final
                                                     competency/certification
                                                     decision
  -----------------------------------------------------------------------------

> The 30/70 split is a **Skill2Cred design decision**, not an official
> NCVET/PMKVY weighting.

## Key Features

### 1. Vernacular Voice Assessment

Candidates can demonstrate knowledge through spoken responses instead of
relying entirely on written tests.

-   Hindi / Marathi voice interaction
-   Indic speech-to-text
-   Structured viva questions
-   Experience-based questioning
-   Knowledge and decision-making assessment
-   Voice integrity support

### 2. Practical Skill Assessment

Candidates demonstrate trade-specific skills using structured tasks and
observable performance criteria.

Possible evidence includes:

-   Guided task checklists
-   Tool-use verification
-   Digital tool simulations
-   Image/video evidence
-   Safety checks
-   Assessor observations

Initial demonstration trades can include:

-   Automotive
-   CNC / Machining
-   Solar
-   Electrician
-   Welder

### 3. AI-Assisted Computer Vision

Computer vision can support practical assessment and workplace safety
verification.

``` text
Camera / Image
      ↓
Computer Vision Model
      ↓
PPE / Safety Detection
      ↓
Assessment Evidence
      ↓
Assessor Review
```

The AI provides supporting evidence; it does not independently certify
the candidate.

### 4. Assessment Integrity

Skill2Cred can incorporate mechanisms to reduce proxy and impersonation
attempts:

-   Voice liveness
-   Speaker verification
-   Speaker diarization
-   Session-level identity checks
-   Evidence timestamps
-   Assessor verification

### 5. AI Competency Mapping

Candidate evidence is mapped against relevant:

-   Qualification Packs (QPs)
-   National Occupational Standards (NOS)
-   NSQF-aligned competency requirements
-   Performance criteria

``` text
Candidate Evidence
        ↓
Relevant QP / NOS
        ↓
Competency Mapping
        ↓
Met Competencies + Skill Gaps
```

### 6. Skill Bridge & Retest

If a candidate does not meet the required competency level, Skill2Cred
can identify specific gaps rather than requiring complete retraining.

``` text
Assessment
    ↓
Skill Gap Detection
    ↓
Targeted Micro-Learning
    ↓
Quick Retest
    ↓
Updated Competency Profile
```

The proposed **12-hour Skill Bridge** is a Skill2Cred design component
for targeted remediation.

### 7. Human-in-the-Loop Certification

**AI can:**

-   Assist evidence collection
-   Transcribe voice responses
-   Detect safety/PPE indicators
-   Assist scoring
-   Map evidence to competencies
-   Highlight skill gaps
-   Generate assessment summaries

**Human assessors:**

-   Review evidence
-   Resolve ambiguous cases
-   Validate practical performance
-   Override incorrect AI suggestions
-   Approve the final competency decision
-   Authorize certification

**AI assists. The assessor decides.**

### 8. Verifiable Digital Credentials

Successful candidates can receive digitally verifiable competency
credentials using:

-   W3C Verifiable Credentials
-   JSON-LD
-   Ed25519 signatures
-   QR-based verification

``` text
Credential
    ↓
Digital Signature
    ↓
QR Code
    ↓
Employer / Institution
    ↓
Credential Verification
```

## Offline-First Design

Skill2Cred is designed for assessment locations where internet
connectivity may be unreliable.

``` text
Assessment Starts
      ↓
Local Data / Cache
      ↓
Assessment Continues Offline
      ↓
Evidence Stored Locally
      ↓
Connectivity Restored
      ↓
Secure Synchronization
      ↓
Cloud Records Updated
```

## Target Users

### Workers

-   Informal workers
-   Experienced technicians
-   Apprentices
-   Helpers progressing toward skilled roles
-   Workers seeking formal recognition

### Assessors

-   RPL assessors
-   Skill-centre evaluators
-   Training institutions

### Employers

-   MSMEs
-   Manufacturing organizations
-   OEMs
-   Apprenticeship recruiters

### Government / Skill Ecosystem

-   MSDE ecosystem
-   NCVET ecosystem
-   Skill development institutions
-   ITIs and training centres

## System Architecture

``` text
┌─────────────────────────────────────────────┐
│                 USER LAYER                  │
│ Candidate • Assessor • Employer • Admin     │
└──────────────────────┬──────────────────────┘
                       ↓
┌─────────────────────────────────────────────┐
│             ASSESSMENT LAYER                │
│ Vernacular Viva • Practical Tasks • Evidence│
└──────────────────────┬──────────────────────┘
                       ↓
┌─────────────────────────────────────────────┐
│                 AI LAYER                    │
│ ASR • Computer Vision • Scoring • Mapping   │
└──────────────────────┬──────────────────────┘
                       ↓
┌─────────────────────────────────────────────┐
│           COMPETENCY ENGINE                 │
│ QP • NOS • NSQF • Skill Gap Analysis        │
└──────────────────────┬──────────────────────┘
                       ↓
┌─────────────────────────────────────────────┐
│              REMEDIATION                   │
│ Skill Bridge • Micro-Learning • Retest      │
└──────────────────────┬──────────────────────┘
                       ↓
┌─────────────────────────────────────────────┐
│               TRUST LAYER                   │
│ Human Approval • W3C VC • Ed25519 • QR      │
└─────────────────────────────────────────────┘
```

## Technology Stack

### Frontend

-   Next.js 16
-   React 19
-   TypeScript
-   Progressive Web App (PWA)

### AI & Computer Vision

-   Python
-   Indic ASR / Indian-language speech models
-   YOLOv8
-   AI-assisted scoring and competency mapping

### Backend / Application

-   Node.js
-   API-based service architecture
-   Authentication and role-based workflows

### Data

-   PostgreSQL
-   Prisma ORM

### Credentials & Trust

-   W3C Verifiable Credentials
-   JSON-LD
-   Ed25519
-   QR verification

## Assessment Workflow

### Step 1 --- Candidate Onboarding

The candidate provides:

-   Basic profile
-   Previous work experience
-   Trade / occupation
-   Preferred language
-   Existing certificates, if any
-   Relevant work history

### Step 2 --- Vernacular Viva

The system:

1.  Captures voice
2.  Converts speech to text
3.  Analyzes responses
4.  Records evidence
5.  Produces an AI-assisted score

### Step 3 --- Practical Evaluation

The candidate performs trade-specific tasks while the platform records:

-   Task completion
-   Observable criteria
-   Safety/PPE indicators
-   Evidence
-   Assessor observations

### Step 4 --- Competency Mapping

Evidence is compared with relevant QP/NOS requirements.

``` text
✓ Competency A
✓ Competency B
✓ Competency C
△ Competency D
✗ Competency E
```

### Step 5 --- Skill Bridge

Missing competencies are converted into targeted learning and a quick
retest.

### Step 6 --- Certification

The authorized assessor reviews the complete evidence package.

``` text
Candidate
   ↓
Competency Profile
   ↓
Assessor Approval
   ↓
Verifiable Credential
   ↓
QR Verification
```

## Human + AI Decision Boundary

  Decision                         AI   Human
  ------------------------------- ---- -------
  Speech transcription             ✓   
  PPE detection                    ✓   
  Evidence organization            ✓   
  Competency mapping assistance    ✓      ✓
  Score recommendation             ✓      ✓
  Ambiguous evidence                      ✓
  Final competency decision               ✓
  Certification approval                  ✓

## Security & Privacy Principles

Skill2Cred is designed around:

-   Role-based access
-   Secure authentication
-   Encrypted communication
-   Minimal collection of personal data
-   Controlled access to assessment evidence
-   Signed credentials
-   Audit trails
-   Human review of high-impact decisions

Voice or biometric information, where used, should be handled according
to applicable consent, privacy and data-retention requirements.

## Research & Standards

The project is informed by:

-   **NCVET** --- Recognition of Prior Learning Guidelines
-   **MSDE** --- PMKVY 4.0
-   **NITI Aayog** --- informal employment / PLFS analysis
-   **NSDC** --- Qualification Packs and National Occupational Standards
-   **AI4Bharat** --- Indian-language speech technology
-   **W3C** --- Verifiable Credentials
-   **OECD** --- RPL assessment quality and reliability research

## Impact

``` text
Informal Experience
        ↓
Recognized Competence
        ↓
Formal Credential
        ↓
Employer-Verified Skill
        ↓
Better Employment Opportunities
```

### Social

-   Makes existing skills visible
-   Reduces language barriers
-   Supports recognition of informal workers
-   Creates clearer career progression

### Economic

-   Reduces unnecessary repeat training
-   Helps employers identify verified skills
-   Improves portability of competency evidence
-   Supports faster skill-to-employment pathways

### System

-   Structured assessment evidence
-   Better assessor consistency
-   Digital verification
-   Scalable RPL workflows
-   Data-driven skill-gap identification

## Future Scope

-   Additional QPs and trades
-   More Indian languages
-   Advanced practical computer vision
-   Improved offline synchronization
-   Employer-side talent discovery
-   Integration with national skill and employment ecosystems
-   Credential wallet integration
-   Longitudinal skill profiles
-   Assessor analytics and calibration

## Project Identity

**Project:** Skill2Cred\
**Tagline:** *From Experience → Evidence → Credential*

**Built for:** Smart India Hackathon 2026

**Problem Area:** AI-Assisted Skill Assessment for Recognition of Prior
Learning (RPL)

## Important Note

Skill2Cred is an AI-assisted RPL prototype/concept. AI-generated scores,
mappings and evidence are intended to **assist authorized assessors**
and should not independently determine certification.

Official policy, qualification standards, assessment requirements and
credential formats should always be validated against the latest
applicable requirements of the relevant authorities.

------------------------------------------------------------------------

## License

Add the project's chosen open-source or proprietary license here before
public release.
