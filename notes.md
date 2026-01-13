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

