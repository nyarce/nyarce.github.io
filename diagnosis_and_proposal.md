# Rancher Onboarding Process: Diagnosis & Proposal

## Executive Summary

The current rancher onboarding process averages 90-120 days from contract signing to Project Start Date. Analysis of the sequential workflow time frames suggests **103 days** for the longest path through the process. Through parallelization, proactive coordination, and dedicated ownership, the proposed process reduces onboarding time to **53 days (49% reduction)**, or **73 days with 20-day contingency buffer (29% reduction)**.

**Current Capacity:** 35.4 ranches/coordinator/year (103-day process)

**Proposed Capacity (Best Case):** 68.9 ranches/coordinator/year (53-day process)

**Proposed Capacity (With Buffer):** 50 ranches/coordinator/year (73-day process)

**Impact:** 94% increase without buffer, or 41% increase with 20-day contingency buffer

---

## 1. Mapping Process

### Assumption
Mapping duration reduced from 10 to 4 days, assuming current delays stem from manual GIS work or shapefile import constraints.

### Questions
- Is the 10-day duration driven by staff capacity limitations or technical restrictions?
- Does the Map Specialist team have bandwidth to handle faster turnaround times?
- Are there existing automation capabilities within PastureMap that aren't being utilized or should be developed in anticipation of growth?

### Risks
- If mapping delays are due to staff capacity constraints (not technical limitations), reduction to 4 days may not be achievable without additional support
- Automated boundary detection may require initial investment in satellite imagery tools or subscriptions
- Self-service mapping by ranchers could introduce quality control issues requiring additional QA time

### Optimization Opportunities
- **Implement automated boundary detection using satellite imagery:** Leverage modern tools for boundary detection from satellite data, reducing manual GIS work
- **Request existing shapefiles/property boundaries during the sales cycle (pre-contract):** Sales team collects ranch boundary data during contract negotiation, enabling mapping to begin immediately upon contract signature
- **Leverage PastureMap's existing capabilities:** GRC owns PastureMap with 30K+ users - explore if self-service mapping features already exist or would provide value during sales closing

---

## 2. Parallelized Processes

### Assumption
Soil sampling and GMP consultation can run in parallel, as GMP planning does not require soil test results to begin.

### Questions
- Does the GMP consultation rely on soil sampling results as a go/no-go decision point?
- Can Understanding Ag begin GMP planning with only mapped ranch data, or are soil results required?
- What is the typical lead time for booking EarthOptics and Understanding Ag appointments?

### Risks
- **Critical Dependency Risk:** If soil results are required before GMP can proceed, an additional 20 days must be added to the timeline (53 → 73 days before buffer), reducing time savings significantly
- Third-party vendor availability may not align with proposed timeline if booking occurs reactively
- Rancher availability unpredictability (calving season, weather, busy periods) could delay both tracks if not proactively managed

### Optimization Opportunities
- **Proactive Scheduling During Sales Cycle:**
  - Sales team collects rancher scheduling availability (seasonal constraints, calving periods, weather windows) during contract negotiation
  - Scheduling data included in handoff package to Rancher Coordinator
  - Enables proactive coordination with third-party vendors (EarthOptics, Understanding Ag) before contract signing
- **Pre-book appointments on Day 0:** With scheduling data from Sales, coordinator can book soil sampling and GMP consultation immediately upon contract signature provided Map Results are reliably delivered
- **Reduce coordination time from 20 days to 0 days:** Eliminate reactive back-and-forth scheduling by frontloading availability collection

---

## 3. Rancher Training

### Assumption
PastureMap training can be split into two phases to improve retention and accelerate onboarding.

### Questions
- Would a staged training approach improve rancher engagement and reduce time-to-productivity?
- What is the current training format (duration, delivery method, content)?
- Do ranchers currently experience low retention or confusion when training happens after long delays?

### Risks
- Splitting training into two phases may require additional PastureMap Specialist time compared to single-session training
- Ranchers may not prioritize Phase 1 training (sample data) if they don't yet have their own ranch data
- If Phase 1 training is skipped, the time savings disappear

### Optimization Opportunities
- **Phase 1 - Initial Training (Available Anytime):**
  - Introduce ranchers to PastureMap using sample training data, covering basic navigation, features, and functionality
  - Can be delivered asynchronously (recorded video) or scheduled early in the process
  - Keeps rancher engaged during the 34-day soil/GMP parallel phase
- **Phase 2 - Applied Training (Post-GMP Delivery):**
  - Schedule training near completion of GMP consultation using rancher's actual property data for immediate application
  - Improves retention by allowing ranchers to apply learning to their specific operation
  - Reduces "time to productivity" by enabling ranchers to start using PastureMap sooner

---

## 4. Dedicated Rancher Coordinator

### Assumption
A dedicated Rancher Coordinator serves as the central hub for all communication between third-party consultants (EarthOptics, Understanding Ag), internal teams, and the rancher.

### Questions
- Does the current Rancher Coordinator role have capacity and authority to own end-to-end onboarding?
- How many ranches is a Rancher Coordinator currently managing concurrently?
- What tools/systems do coordinators currently use for tracking and communication?

### Risks
- Coordinator role may become a bottleneck if one person is responsible for too many concurrent ranches without proper tooling
- Without clear authority, coordinators may still need to defer to other teams for decisions, reintroducing handoff delays
- If coordinators lack visibility into third-party vendor status, they cannot proactively manage timelines

### Optimization Opportunities
- **Single Point of Contact:** Eliminate confusion and delays caused by unclear handoff ownership - rancher has one consistent contact throughout the entire onboarding journey
- **Coordinator as Project Manager:** Coordinator owns all deliverables, handoffs, and communications from contract signature to Project Start Date
- **Implement project management platform (Monday.com or ClickUp) with automated task generation:**
  - Contract signed → Auto-create ranch onboarding project from template
  - Task completion triggers next-step assignments and deadline recalculations
  - Dependency-based deadline adjustments (if soil sampling delayed → Project Start Date auto-adjusts)
- **Enable real-time deadline tracking, dependency management, and visibility dashboards:**
  - Coordinator sees all 10 concurrent ranches in one dashboard with color-coded status indicators (on track, at risk, blocked)
  - Multi-view options: List, Board (Kanban), Timeline (Gantt), Calendar
- **Capacity Impact:** At 53 days per cohort, each Rancher Coordinator can manage 6.887 cohorts/year × 10 ranches = 68.9 ranches annually (94% increase from 35.4 ranches/year). With 20-day contingency buffer (73 days), capacity is 5.0 cohorts/year × 10 ranches = 50 ranches annually (41% increase)

---

## Contingency Planning

### Buffer: 20-30 Days
Adding a contingency buffer brings total timeline to **73-83 days**.

**Buffer Accounts For:**
- Potential dependency if GMP consultation requires soil results (+20 days)
- Implicit buffer in original 120-day estimate (120 vs 103 calculated = 17 days)
- Third-party coordination unpredictability (weather, resource availability)

**With 20-day buffer (73 days total):**
- 30 days faster than current calculated process (103 days) = 29% improvement
- 47 days faster than original estimate (120 days) = 39% improvement

**Even with 30-day buffer (83 days total):**
- 20 days faster than current calculated process (103 days) = 19% improvement
- 37 days faster than original estimate (120 days) = 31% improvement

---

## Implementation Priority

**Phase 1 (Quick Wins - Low Risk):**
1. Proactive scheduling data collection during sales cycle
2. PM platform (Monday.com or ClickUp) template setup with standardized ranch onboarding workflow
3. Establish single Rancher Coordinator as owner for each ranch

**Phase 2 (High Impact - Requires Validation):**
1. Validate GMP/soil dependency assumption with Understanding Ag
2. Implement parallelization of soil sampling and GMP consultation
3. Optimize mapping process (shapefiles collection, automation exploration)

**Phase 3 (Long-term Optimization):**
1. Staged rancher training approach (Phase 1 and Phase 2 split)
2. Automated task generation and deadline recalculation in PM platform
3. Integration with Salesforce, calendar tools, and communication platforms
