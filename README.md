# MinuteFlow — AI Meeting Notes to Action Items

An AI-powered meeting productivity application built using **Google AI Studio Build mode and Gemini**.

MinuteFlow transforms rough meeting notes into structured summaries, decisions, action items, and follow-up emails. It also includes a source-review checkpoint to help users verify AI-generated information against the original meeting notes before copying or sharing outputs.

## Project Overview

Professionals often need to spend additional time converting meeting discussions into actionable follow-ups.

MinuteFlow explores how an AI-powered application can simplify this workflow while maintaining factual accuracy, privacy awareness, and human oversight.

**Project:** Meeting Notes to Action Items  
**Built with:** Google AI Studio Build mode and Gemini  
**Development:** October 2026  
**Status:** Completed and published

## Key Features

- **Meeting Summaries:** Convert rough meeting notes into structured summaries.
- **Decision Tracking:** Extract and organise decisions discussed during meetings.
- **Action Item Extraction:** Identify tasks, owners, deadlines, and relevant notes.
- **Follow-up Email Generation:** Create follow-up emails using Friendly, Concise, and Formal tone options.
- **Source Review:** Compare generated action items against the original meeting notes.
- **Human Verification:** Require confirmation of the generated information before unlocking action-item and email copy controls.

## Responsible AI and Reliability

An important part of this project was improving the reliability of AI-generated outputs.

During testing, I identified an issue where the application incorrectly assigned an unspecified action owner and repeated an embedded instruction from adversarial meeting notes.

I refined the application to address these issues:

- Missing owners are identified as "Not specified" rather than inferred.
- Embedded instructions in meeting notes are not treated as valid instructions.
- Generated outputs must be checked against the original source notes.
- Copy controls remain unavailable until the user confirms the source review.

This introduced a human-in-the-loop verification step before sharing generated outputs.

## Testing and Validation

I tested MinuteFlow using clear, incomplete, vague, and adversarial fictional meeting notes.

Testing included:

- Verifying summaries against original meeting notes.
- Checking decisions, action owners, and deadlines.
- Comparing outputs across all three email tones.
- Identifying incorrect assumptions and missing information.
- Verifying source-review controls before and after confirmation.
- Testing the published application in Safari Private Browsing without signing in to Google.

The final verification confirmed that the application preserved the tested meeting facts and enforced the source-review checkpoint.

## Tools and Concepts

**Tools**
- Google AI Studio Build mode
- Gemini
- Google AI Studio application preview

**Concepts explored and applied**
- Prompt engineering
- Vibe coding
- Structured AI outputs
- Iterative application development
- Factual grounding
- Adversarial input testing
- Human-in-the-loop review
- Responsible AI design

## Project Impact — Illustrative Estimate

Based on a synthetic workflow using fictional meeting notes, I estimated that manually preparing the meeting summary, decision log, action-item table, and follow-up email could take approximately 10–15 minutes.

The application workflow was recorded at 1.99 seconds, including review.

Using an illustrative assumption of 10 meetings per week, the estimated potential time saving was approximately 125 minutes per week.

*This is an illustrative estimate, not a measured business outcome.*

## Application

The application was published using Google AI Studio.

**Live Demo:** https://minuteflow-meeting-notes-to-action-items.ai.studio

## Project Documentation

The development journey, testing evidence, identified issues, improvements, and final validation are documented in the project report.

[View Project Documentation](docs/Build-Meeting-Actions-in-AI-Studio.pdf)

## Key Learning

This project helped me understand that building a useful AI application involves much more than generating an initial prototype.

Testing incomplete and adversarial inputs, identifying reliability issues, refining prompts, and introducing human verification were equally important parts of the development process.

My next learning goal is to build more advanced AI applications using APIs, Python, and automation tools.
