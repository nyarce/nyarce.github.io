# Part 2: Proposal - Streamlined Onboarding Process

## Overview
The proposed process reduces onboarding time from **103 days to 53 days** (49% reduction), or **73-83 days with contingency buffer** (29-39% reduction). This is achieved through parallelization, proactive coordination, and dedicated ownership.

---

## Proposed Timeline: 53 Days (Base Case)

### Step-by-Step Breakdown

| Step | Owner | Duration | Start Day | End Day | Dependencies |
|------|-------|----------|-----------|---------|--------------|
| Contract Signed | Sales | Day 0 | 0 | 0 | - |
| Ranch Mapped in PastureMap | Map Specialist | 4 days | 0 | 4 | Contract signed |
| Soil Sampling Scheduled | Rancher Coordinator | 20 days | 0 | 20 | Pre-scheduled during sales |
| Soil Sampling Completed | EarthOptics (3rd party) | 14 days | 20 | 34 | Scheduled appointment |
| GMP Consultation | Understanding Ag (3rd party) | 30 days | 4 | 34 | Mapped ranch |
| GMP Delivered to Rancher | Grazing Engineer | 14 days | 34 | 48 | Consultation complete |
| Rancher Trained on PastureMap | PastureMap Specialist | 10 days | 42 | 52 | Overlaps with GMP delivery |
| Project Start Date Established | MRV Team | 5 days | 48 | 53 | All above complete |

### Key Changes from Current State:
- **Mapping reduced from 10 → 4 days** (automated boundary detection, pre-contract shapefile collection)
- **Soil sampling and GMP run in parallel** (Day 0-34 for soil, Day 4-34 for GMP)
- **Training overlaps with GMP delivery** (Day 42-52 instead of waiting until Day 88)

---

## 1. Which Steps Can Be Parallelized

### Primary Parallelization: Soil Sampling + GMP Consultation
**Current:** Sequential (soil → GMP) = 44 days
**Proposed:** Parallel (both run simultaneously) = 34 days
**Savings:** 10 days

**Critical Assumption:** GMP consultation does not require soil test results as a go/no-go decision point. If soil results are required, add 20 days back to timeline.

**Why This Works:**
- GMP planning focuses on grazing strategies, pasture rotation, and management practices
- Soil data provides supplementary information for carbon baseline but isn't needed to begin consultation
- Both processes can start once ranch is mapped

### Secondary Parallelization: Training Overlap
**Current:** Training starts after GMP delivery (Day 88)
**Proposed:** Training overlaps with GMP delivery (Day 42-52)
**Savings:** 10 days removed from critical path

**Why This Works:**
- Phase 1 training (sample data) can happen early in the process
- Phase 2 training (applied to actual ranch data) happens near GMP completion for better retention

---

## 2. Where Handoff Ownership Should Sit

### Dedicated Rancher Coordinator as End-to-End Project Manager

**Current Model Issues:**
- Handoffs between Sales, Map Specialist, Coordinator, Third-parties, Training, MRV
- No single owner for the rancher's journey
- Tasks stall between steps with unclear responsibility

**Proposed Model:**
**One Rancher Coordinator** owns the entire onboarding journey from contract signature to Project Start Date.

**Responsibilities:**
- ✅ Receives handoff package from Sales with pre-collected scheduling data
- ✅ Submits mapping request to Map Specialist and monitors completion
- ✅ Coordinates with EarthOptics for soil sampling (using pre-collected availability)
- ✅ Coordinates with Understanding Ag for GMP consultation
- ✅ Schedules PastureMap training at optimal timing
- ✅ Monitors all dependencies and escalates blockers
- ✅ Serves as single point of contact for rancher throughout process
- ✅ Triggers MRV team when all deliverables are complete

**Capacity Impact:**
At 53 days per cohort, each Rancher Coordinator can manage:
- 365 days/year ÷ 53 days/cohort = 6.887 cohorts/year
- 6.887 cohorts × 10 ranches/cohort = **68.9 ranches annually**
- Current capacity: 35.4 ranches/coordinator/year (103-day process)
- **Improvement: 94% increase in capacity without adding headcount**

---

## 3. Tracking & Visibility Mechanism

### Proposed Tool: ClickUp (or similar PM platform)

**Core Features:**
1. **Standardized Ranch Onboarding Template**
   - Pre-configured task list for all 8 steps
   - Dependency mapping (soil sampling → Project Start Date)
   - Automatic deadline calculations based on contract signature date

2. **Automated Task Generation**
   - Contract signed → Create ranch project from template
   - Ranch mapped → Trigger soil sampling coordination task
   - GMP complete → Schedule training task

3. **Multi-Ranch Dashboard**
   - Coordinator views all 10 concurrent ranches in one place
   - Color-coded status indicators (on track, at risk, blocked)
   - Timeline view showing parallel processes across ranches

4. **Dependency-Based Deadline Adjustments**
   - If soil sampling is delayed by 5 days → Project Start Date auto-adjusts +5 days
   - If GMP completes early → Training task deadline moves up automatically

5. **Automated Notifications**
   - Task completion triggers next-step assignments
   - 3-day reminders before third-party appointments
   - Escalation alerts for tasks overdue by >2 days

**Why ClickUp:**
- Native support for task templates and dependencies
- Automation rules without coding (vs. building custom solution)
- API integrations with CRM (for contract data) and communication tools (Slack/Email)
- Cost: ~$19/user/month (vs. $50K+ to build custom)

---

## 4. Third-Party Coordination Challenge

### Strategy: Proactive Scheduling During Sales Cycle

**Current Problem:**
- Coordinator reaches out to third-parties reactively after mapping complete
- Back-and-forth scheduling with rancher causes 10-20 day delays
- No visibility into seasonal constraints (calving, weather windows)

**Proposed Solution:**
**Sales team collects scheduling data during contract negotiation:**
- Rancher's seasonal availability (calving periods, busy seasons)
- Weather windows for soil sampling
- Preferred contact times and communication methods
- Property access constraints

**Handoff Package to Coordinator includes:**
- Signed contract
- Ranch boundary shapefiles (if available)
- Scheduling availability matrix
- Third-party vendor preferences (if any)

**Coordinator Actions (Day 0):**
- Submit mapping request (using pre-collected shapefiles)
- Pre-book soil sampling appointment with EarthOptics (using scheduling matrix)
- Pre-book GMP consultation slot with Understanding Ag (using seasonal availability)

**Result:**
- Third-party appointments locked in before mapping even starts
- Reduces scheduling coordination from 20 days → 0 days (pre-booked during sales)
- Rancher feels "VIP treatment" with proactive communication

---

## 5. Tools to Buy vs. Build

### Recommended: Buy (Don't Build)

**Primary Tool: ClickUp ($19/user/month)**
- Project management platform with native automation
- Task templates, dependencies, and deadline adjustments
- Multi-ranch dashboard for coordinators

**Integrations (via ClickUp API):**
- **CRM integration**: Contract signed → auto-create ClickUp project
- **Calendar integration**: Third-party appointments sync to ClickUp timeline
- **Communication**: Slack/Email notifications for task updates

**Secondary Tools:**
- **PastureMap**: Already owned by GRC for ranch mapping (leverage self-service features)
- **Calendly/Acuity**: Third-party scheduling links embedded in coordinator workflows
- **Zapier/Make**: No-code automation between ClickUp, CRM, and communication tools

**Build vs. Buy Decision:**
- **Build:** $50-100K development + ongoing maintenance
- **Buy:** ~$2,000/year for 10 coordinators + integrations
- **Time to Deploy:** 2-4 weeks (ClickUp setup) vs. 6-12 months (custom build)

---

## Contingency Planning

### 20-30 Day Buffer
Adding a contingency buffer brings total timeline to **73-83 days** (still 20-39% faster than current 103 days).

**Buffer Accounts For:**
1. **GMP/Soil Dependency Risk:** If GMP consultation requires soil results, add 20 days
2. **Implicit Buffer Matching:** Original 120-day estimate vs. 103-day calculated = 17-day buffer
3. **Weather/Availability Delays:** Third-party coordination unpredictability

**Even with maximum buffer (83 days):**
- 20 days faster than current process (103 days)
- 37 days faster than original estimate (120 days)
- 19% improvement vs. current state

---

## Summary

The proposed process achieves a **49% reduction in onboarding time** through:
1. ✅ **Parallelization** of soil sampling and GMP consultation (saves 10 days)
2. ✅ **Dedicated ownership** by single Rancher Coordinator (eliminates handoff delays)
3. ✅ **Proactive scheduling** during sales cycle (saves 10-20 days)
4. ✅ **Strategic training timing** (removes 10 days from critical path)
5. ✅ **Automated tracking** via ClickUp (visibility and dependency management)

With contingency padding, the process delivers a **29-39% improvement** while maintaining realistic buffer for operational uncertainty.
