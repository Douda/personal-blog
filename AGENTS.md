# AGENTS.md - Project Guide for AI Assistants

## Tech Stack

- **Static Site Generator**: Hugo (v0.154.2+)
- **Theme**: hugo-blog-awesome
- **Hosting**: GitHub Pages
- **Deployment**: GitHub Actions (automated CI/CD)
- **Repository**: https://github.com/Douda/personal-blog
- **Domain**: boumanne.fr / www.boumanne.fr

## Project Purpose

This blog serves as a marketing and branding platform for Aurélien BOUMANNE's cloud engineering journey. It documents progression through professional certifications and hands-on projects starting in 2025.

### Primary Goals:

1. **Professional visibility** - Establish credibility in cloud computing and DevOps
2. **Learning documentation** - Track progress through AWS, Kubernetes, and Terraform certifications
3. **Community engagement** - Share knowledge and connect with other cloud practitioners
4. **Portfolio building** - Demonstrate practical skills through project write-ups

### Training Path (2026):

The blog chronicles the Cloud Mastery Bootcamp journey, targeting these certifications:
- AWS Certified Solutions Architect Associate
- AWS Certified Developer Associate
- AWS Certified CloudOps Engineer Associate
- Certified Terraform Associate

Previously completed:
- AWS Certified Cloud Practitioner
- Kubernetes and Cloud Native Associate (KCNA)

## Content Tone and Style

### Writing Guidelines:

- **Professional yet approachable** - Technical accuracy without unnecessary jargon
- **Direct and actionable** - Focus on practical insights and lessons learned
- **Transparent** - Share both successes and challenges encountered
- **Forward-looking** - Emphasize continuous learning and growth

### Avoid:
- Excessive emojis or casual language
- Overly promotional or salesy content
- Vague statements without technical backing

## Post Types

### 1. Progress Updates (Short Form)

Brief posts documenting milestones, certification completions, or quick insights.

**Characteristics:**
- 200-400 words
- Single topic focus
- Quick read (2-3 minutes)
- Minimal technical depth

**Example topics:**
- "Passed AWS Solutions Architect Associate"
- "Week 1: Terraform Basics Completed"
- "Key Takeaway from Today's Lab"

**Structure:**
```markdown
---
title: "Brief, descriptive title"
date: YYYY-MM-DD
tags: ["relevant", "tags"]
categories: ["updates"]
---

## What Happened
Brief context or milestone

## Key Insight
Main learning or takeaway

## Next Steps
What's coming next
```

### 2. Technical Deep Dives (Long Form)

Detailed posts covering projects, labs, or in-depth technical explorations.

**Characteristics:**
- 800-2000+ words
- Multiple sections with clear structure
- Code examples and diagrams when relevant
- Thorough technical explanation
- Lessons learned section

**Example topics:**
- "Building a Kubernetes Cluster on Raspberry Pi"
- "Terraform Module for AWS VPC Setup"
- "Implementing CI/CD with GitHub Actions"
- "Multi-Region AWS Architecture Design"

**Structure:**
```markdown
---
title: "Descriptive technical title"
date: YYYY-MM-DD
tags: ["technology", "specific", "tags"]
categories: ["projects"]
description: "Brief summary for SEO"
---

## Overview
Problem statement and objectives

## Background
Context and requirements

## Implementation
Technical details, architecture decisions, code snippets

## Challenges and Solutions
Issues encountered and how they were resolved

## Results
Outcomes and metrics

## Lessons Learned
Key takeaways and best practices

## Next Steps
Future improvements or related work
```

## Content Creation Assistance

When helping create blog posts:

1. **For progress updates**: Keep it concise, focus on the milestone, extract one key learning
2. **For technical posts**: 
   - Start with clear problem definition
   - Include architecture or workflow diagrams (describe them if cannot generate)
   - Provide actual code snippets with explanations
   - Always include a "Lessons Learned" section
   - Link to relevant documentation or resources

3. **General guidelines**:
   - Use clear, professional language
   - Include relevant tags for discoverability
   - Ensure technical accuracy
   - Focus on practical value for readers
   - Maintain consistency with existing content tone

## Repository Structure

```
personal-blog/
├── content/
│   ├── posts/          # Blog articles (markdown)
│   ├── about.md        # About page
│   └── contact.md      # Contact page
├── static/
│   ├── CNAME           # Custom domain configuration
│   └── css/            # Custom styling
├── themes/
│   └── hugo-blog-awesome/  # Theme submodule
├── .github/
│   └── workflows/
│       └── deploy.yml  # Automated deployment
├── config.toml         # Hugo configuration
└── README.md          # Technical documentation
```

## Creating New Posts

```bash
# Short update
hugo new posts/updates/brief-title.md

# Technical deep dive
hugo new posts/projects/detailed-technical-title.md
```

## Deployment Workflow

1. Create or edit markdown files in `content/posts/`
2. Commit changes to main branch
3. GitHub Actions automatically builds and deploys
4. Site updates at www.boumanne.fr within 1-2 minutes

## Brand Voice Summary

**Aurélien BOUMANNE** is a cloud engineering professional documenting his certification journey and hands-on projects. The blog reflects:

- Technical competence without arrogance
- Genuine learning process, including mistakes
- Practical, actionable insights
- Professional growth mindset
- Community contribution focus

The tone is that of an experienced professional leveling up in cloud technologies, sharing the journey transparently to help others and build professional credibility.
