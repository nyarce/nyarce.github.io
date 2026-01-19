# Notes - Grassroots Carbon Interview Prep

## Session 1 Queries (Previous Session)

### Setup & Initial Planning
- Requested two tracking documents: summary.md for query/response tracking, notes.md for links/references
- Wanted to upload resume and practical interview Part 1, then rubber duck ideas and approaches

### Initial Analysis
- Shared first thoughts on bottlenecks: parallelization opportunities, handoff ownership gaps, lack of standardized tracking
- Identified potential for using Sales/established contact as single point of coordination for rancher
- Questioned GMP consultation timeline (7-14 days delivery after 15-30 day consult)
- Noted need for more information from Grassroots to make better decisions

### Capacity & Bottleneck Deep Dive
- Raised concern about Map Specialist capacity: "Should it take a GIS specialist 5-10 days to map a ranch? If a Ranch Coordinator can handle 10 concurrent ranches, can the Map Specialist keep up?"
- Identified potential staffing/capacity bottleneck in mapping process

### Visualization & Refinement
- Requested Gantt chart tool to visualize current process flow and identify parallelization opportunities
- Multiple iterations refining Gantt chart specifications:
  - Map current state with longest timelines (103 days worst case)
  - Remove critical path coloring, focus on Internal vs Third-Party
  - Correct categorization (Soil Sampling = Internal, GMP = Third-Party)
  - Validate sequential timeline math (confirmed 103 days)

### Proposed State Design
- Specified revised timeline reducing 103 days → 53 days:
  - Ranch mapping: 4 days (self-service during sales + QA)
  - Soil sampling: 20 days scheduled, 14 days completion (parallel)
  - GMP consultation: 30 days starting Day 4 (parallel)
  - Training: 10 days starting Day 42 (overlaps with GMP delivery)
  - Project start: Day 53

### Capacity Calculations
- Requested exact capacity math showing ranches per Ranch Coordinator
- Confirmed capacity increase from 35.4 → 68.9 ranches/coordinator/year (94% increase)

### Meta-Analysis
- Requested document summarizing how Claude was used as a tool
- Wanted clear attribution: which insights were user-driven vs Claude-provided
- Sought to understand split of work for interview transparency

### Professional Communication
- Asked for feedback on draft email to interview contact (Wyatt)
- Questions about SOPs, current tools, and deliverable format preferences

---

## Research Links & References

### GIS & Ranch Mapping Automation
- Modern AgTech tools offer automated boundary detection from satellite imagery
- Self-service rancher tools (mobile apps for boundary drawing)
- Import capabilities from existing farm management systems
- PastureMap (owned by GRC) likely has these capabilities already
- Map Specialist role could shift from "mapper" to "QA reviewer"

### Key Insight
- Grassroots Carbon already owns PastureMap with 30K+ users
- Ranch mapping is highly automatable - industry best practice
- 5-10 day manual mapping is likely legacy process
- Automation could reduce to 1-2 day QA + self-service during sales cycle

---

## Current Session Queries

### Setup & File Organization
- Clarified that gantt_chart.html is now index.html
- All Gantt chart modification requests should be made to index.html
- Plan to expand index.html to include rest of Part 1, then Part 2 and Part 3

### Current State Refinements
- Updated bottlenecks in current state view: removed "Reactive Scheduling" and "Capacity Constraint"
- Added new Bottleneck #4: "Rancher training delayed until all other processes are complete"

### Proposed State - Assumption Cards
- Requested cards below Proposed State to explain assumptions and raise questions
- Card 1 - Mapping Process: Questions staff capacity vs technical restrictions, suggests satellite imagery automation and pre-contract shapefile collection
- Card 2 - Parallelized Processes: Questions if GMP relies on soil results as go/no-go signal, suggests Sales collect scheduling availability for proactive planning
- Card 3 - Rancher Training Opportunities: Proposes staged training approach (Phase 1: sample data anytime, Phase 2: live data post-GMP for better retention)
- Card 4 - Dedicated Rancher Coordinator: Single point of contact for all parties, acts as PM owning deliverables/handoffs, suggests PM tools (ClickUp/Monday.com) for automation

### Proposed State Card Cleanup
- Requested cleanup of the assumption cards displayed under Proposed State view
- Claude identified the 4 cards (Mapping Process, Parallelized Processes, Rancher Training, Dedicated Coordinator) and asked for clarification on specific cleanup needs

### Process Documentation
- Reminded Claude that all prompts need to be summarized and added to notes.md for session tracking

### Mapping Process Card Updates
- Removed "Enable rancher self-service mapping via PastureMap mobile app" bullet point from Further Optimization Opportunities
- Now only includes: automated boundary detection and pre-contract shapefile collection

### Parallelized Processes Card Updates
- Changed "Critical Question:" to "Question:" for consistency with other cards

### Card Formatting Standardization
- Reformatted all four cards to follow consistent structure: Assumption → Question → Further Optimization Opportunities
- **Rancher Training Card**: Condensed Phase 1 and Phase 2 details into two bullet points under opportunities
- **Dedicated Rancher Coordinator Card**: Combined Benefits and Operational Tooling sections into single opportunities list with 5 bullet points

### Contingency Padding Addition
- Added "Contingency Padding" bullet point to Proposed Optimizations section
- Math: 53 days + 20-30 days buffer = 73-83 days total
- Still 20-30 days faster than current 103-day process
- Still 37-47 days faster than originally estimated 120 days
- Accounts for: potential GMP/soil dependency (+20 days) and matches implicit buffer in original estimate (120 vs 103 = 17 days)
- Removed redundant "Math:" bullet point from sub-list

### Requirements Review
- Shared full Part 1 requirements to verify deliverables and assess if work is overdone
- Requested analysis of what's been built vs. what's required and recommendations for Part 2
- Analysis showed: Diagnosis ✅ and Proposal ✅ are covered by assumption cards and Gantt charts, but Playbook ❌ is missing

### ClickUp Implementation Plan
- Decided to implement ClickUp as the proposed PM tool for the "Propose" section
- Key features: standard templates for ranch onboarding, automatic deadline adjustments based on task dependencies
- Addresses requirements: tracking/visibility mechanism and tools to buy/build

### Deliverable Creation
- **Created page1_diagnosis.md:** 4-bottleneck analysis with impact assessment and revenue implications
- **Created page2_proposal.md:** Full proposal with parallelization strategy, ownership model, tracking mechanism, third-party coordination, and buy vs. build decision
- **Added third button to index.html:** "ClickUp Implementation" view alongside Current State and Proposed State
- **ClickUp Implementation view includes:**
  - Overview (cost, setup time, alternative costs)
  - Core Features (template, automation, dependency tracking, dashboard, notifications)
  - Automation Examples (5 trigger→action workflows)
  - Dashboard Views (List, Board, Timeline, Calendar, Status indicators)
  - Integrations (CRM, Calendar, Communication, PastureMap)
  - Placeholder section for screenshots and mockups to be added later

### Playbook Draft
- **Created page3_playbook.md:** One-page operational guide for managing 10 concurrent ranches
- Includes sections: Pre-contract handoff, Day 0 actions, weekly monitoring, stage-by-stage workflow, escalation protocols, dashboard views, and tips
- Contains [QUESTION: ...] tags throughout where operational details need to be filled in or verified
- User acknowledged lacking detailed operational knowledge to make playbook fully accurate - draft created for review and editing

### Current State Bottleneck Reordering
- Swapped bottlenecks to follow sequential process order:
  - #1: Manual Ranch Mapping (was #2) - happens first in process
  - #2: Sequential Dependencies (was #1) - happens during soil/GMP phase
  - #3: Rancher Training Delayed (was #4) - happens at end of process
  - #4: No Single Owner (was #3) - cross-cutting issue throughout

### Combined Diagnosis & Proposal Document
- **Created diagnosis_and_proposal.md:** Single document combining diagnosis and proposal sections
- Structured using the 4 assumption cards as the outline (Mapping Process, Parallelized Processes, Rancher Training, Dedicated Rancher Coordinator)
- Each section formatted consistently: Assumption → Questions → Risks → Optimization Opportunities
- Includes: Executive Summary with capacity impact, detailed sections for each optimization area, Contingency Planning, and Implementation Priority phases
- User will review and edit to match their voice and add missing details

### Tool Selection Discussion
- Debated ClickUp vs Monday.com as PM platform
- Recommendation: Monday.com for better non-technical user experience, easier onboarding, superior visualization
- User considering whether to create Monday.com mockup (may be excessive for interview deliverable)

### Simplified Playbook
- **Replaced page3_playbook.md with playbook.md:** Simplified one-page format following Option 2 approach
- Structure: 6 Operating Principles + Dashboard View description + Weekly Workflow + Success Metrics + Tools/Integrations
- Principles-based rather than step-by-step instructions
- Includes table showing Kanban board structure with color-coded status indicators
- User may add Monday.com mockup screenshot if desired

### PM Platform & Automation Tab Updates
- **Renamed "ClickUp Implementation" to "PM Platform & Automation"** - allows discussion of both Monday.com and ClickUp
- Updated button and function names (showPMTools, currentView = 'pmtools')
- **Added Tool Comparison section:** Side-by-side comparison of Monday.com vs ClickUp with costs and tradeoffs
- **Added visual Automation Flow diagram:** Step-by-step color-coded flow showing:
  - Salesforce trigger (Closed Won → Create board)
  - Day 0 automations (mapping, soil, GMP)
  - Mapping complete trigger
  - Parallel execution tracking (Day 4-34)
  - Convergence point (both soil & GMP done)
  - Final step (training → project start date)
  - Escalation rules
- **Added Salesforce Data Transfer card:** Explains what data can/cannot transfer from Salesforce (shapefiles stay in Drive/Dropbox, links transfer)
- Updated all cards to be tool-agnostic (works for both Monday.com and ClickUp)
- 6 cards total: Core Features, Automation Examples, Dashboard Views, Integrations, Salesforce Data Transfer, plus Automation Flow visual

### Cross-Document Consistency Check & Fixes
- **Identified major baseline inconsistencies** across documents
- **Fixed diagnosis_and_proposal.md** to use consistent 103-day baseline:
  - Current: 103 days → 35.4 ranches/year
  - Proposed: 53 days → 68.9 ranches/year (94% increase)
  - With buffer: 73 days → 50 ranches/year (41% increase)
- **Corrected capacity calculations** (Line 116): Fixed from "5 cohorts = 50 ranches (41%)" to "6.887 cohorts = 68.9 ranches (94%)"
- **Updated contingency planning section** with accurate math for both 20-day and 30-day buffers
- **Changed all tool references** from "ClickUp" to "Monday.com or ClickUp" for consistency with other documents
- All documents now aligned on baselines, capacity numbers, and tool recommendations

### Release Notes SOP Addition
- **Added fourth button to index.html:** "Release Notes SOP" view
- Imported and formatted content from /Users/nyarce/Documents/Final-ReleaseNotes.md
- **Formatted sections include:**
  - Purpose statement
  - Release Notes Structure & Templates (3 templates: Sales/Customer, Internal, C-Suite)
  - Distribution Matrix table (showing audience, template, channel, timing, content focus)
  - Workflow & Ownership table (roles, responsibilities, time estimates)
  - Process Steps (5-step workflow)
  - Release Cadence & Exceptions (Hotfixes and Major Releases)
  - Automation recommendations
  - Making It Stick (critical success factors)
  - Quick Reference Checklist (2-column grid with Before Release and Distribution checklists)
- All content styled consistently with existing assumption cards and tables

