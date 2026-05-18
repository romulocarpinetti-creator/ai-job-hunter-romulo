# PRODUCT_SPEC.md

# AI Job Hunter — Product Specification

## Overview

AI Job Hunter is a web application designed to automatically search, analyze and organize remote job opportunities related to generative AI, audiovisual production, creative technology and AI-driven content creation.

The platform is specifically optimized for the professional profile of Rómulo Carpinetti: Creative AI Director, AI Filmmaker and Generative Visual Storyteller.

The system uses AI to:
- search job opportunities,
- evaluate compatibility,
- score job matches,
- generate personalized applications,
- summarize opportunities,
- and organize the entire application workflow.

---

# Core Goals

1. Automatically find remote job opportunities.
2. Analyze compatibility using AI.
3. Generate personalized applications and cover letters.
4. Organize opportunities in a dashboard.
5. Notify the user via email.
6. Save time and improve job search quality.
7. Prioritize high-quality international opportunities.

---

# Primary Job Categories

- Creative AI Director
- AI Filmmaker
- AI Video Creator
- Creative Technologist
- Generative AI Artist
- AI Content Producer
- Prompt Engineer
- AI Visual Storyteller
- Branded Content Specialist
- Generative Video Specialist
- Director creativo IA
- Realizador audiovisual IA

---

# Platforms to Monitor (MVP)

## Priority Platforms
- RemoteOK
- GetOnBoard
- WeRemoto
- Wellfound
- Indeed

## Phase 2 Platforms
- LinkedIn Jobs
- Workana
- Upwork
- Behance Jobs
- Domestika Jobs
- Torre

---

# Technology Stack

## Frontend
- Next.js
- Tailwind CSS
- TypeScript

## Backend
- Next.js API routes
or
- FastAPI (optional future migration)

## Database
- Supabase

## AI Layer
- OpenAI API

## Email
- Resend
or
- Gmail API

## Scraping / Data Collection
- RSS feeds
- Public APIs
- Playwright
- Apify (future)
- Custom scrapers

## Deployment
- Vercel

---

# Main Features

## 1. Job Search Engine

The system should:
- search remote jobs periodically,
- collect title,
- company,
- description,
- location,
- salary if available,
- tags,
- job link,
- date.

Search should prioritize:
- remote jobs,
- AI-related jobs,
- audiovisual and creative opportunities,
- Spanish-speaking countries,
- international remote positions.

---

# 2. AI Job Analysis

Every job listing should be analyzed using OpenAI.

The AI should:
- summarize the opportunity,
- identify required skills,
- calculate compatibility score,
- explain why it matches,
- identify missing skills,
- classify job type.

---

# 3. Job Match Score

Score range:
- 1 to 10

## High Match (9–10)
- Remote
- AI + audiovisual + creative direction
- Strong storytelling or branded content
- Uses AI tools related to video/image generation

## Medium Match (7–8)
- Good creative fit
- Some AI relevance
- Remote or hybrid

## Low Match (Below 6)
- Pure engineering
- No AI relevance
- No creative/audiovisual component
- Non-remote

---

# 4. Personalized Application Generator

The AI should generate:
- cover letters,
- short application messages,
- LinkedIn messages,
- email introductions.

Applications should:
- adapt to job description,
- use MASTER_PROFILE.md as context,
- sound professional and international,
- avoid generic AI wording,
- emphasize audiovisual experience + AI specialization.

---

# 5. Dashboard

The dashboard should display:
- list of jobs,
- compatibility score,
- platform,
- company,
- location,
- status,
- notes,
- generated application.

## Status Types
- New
- Saved
- Applied
- Rejected
- Interview
- Archived

---

# 6. Email Notifications

The system should send:
- daily email summaries,
- top opportunities,
- high-match alerts.

Email includes:
- company,
- role,
- match score,
- short summary,
- direct link.

---

# 7. Filters

Users should filter by:
- remote only,
- salary,
- country,
- language,
- AI category,
- creative category,
- score.

---

# Database Schema

## jobs
- id
- title
- company
- platform
- description
- location
- remote
- salary
- url
- created_at
- ai_summary
- ai_score
- ai_reasoning
- application_generated
- status

## applications
- id
- job_id
- generated_cover_letter
- generated_message
- applied_at
- status

---

# OpenAI Prompts

The app will use:
- MASTER_PROFILE.md
- scoring prompts
- cover letter prompts
- summarization prompts

---

# Future Features

## Phase 2
- LinkedIn scraping
- Upwork integration
- Workana integration
- recruiter tracking
- application automation
- Chrome extension

## Phase 3
- Multi-user SaaS
- Subscription system
- AI recruiter assistant
- Personalized opportunity recommendations
- Portfolio analyzer

---

# UI Style

The interface should feel:
- modern,
- cinematic,
- premium,
- AI-focused,
- minimal-tech,
- editorial-inspired.

Dark mode preferred.

---

# MVP Priority

The first MVP must include:

1. Job scraping/search
2. Supabase database
3. AI scoring
4. Dashboard
5. Generated applications
6. Email notifications

Everything else is secondary.

---

# Important Notes

- The system should avoid violating platform rules.
- Do not automate direct applications in the first version.
- Focus on opportunity analysis and preparation first.
- Prioritize quality over quantity.
- Use AI to reduce manual effort while maintaining personalized applications.
