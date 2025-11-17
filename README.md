# Tasfiya-Learning

# 30-Day Salesforce Developer Learning & Practice Schedule

Assumption: ~3–4 focused hours per day. Maintain a Git repo. Use a Dev Hub + scratch orgs for experimentation; keep one persistent sandbox/dev org for cumulative build.

| Day | Theme | Key Topics | Hands-On Tasks | Output / Artifact | Self-Check |
|-----|-------|------------|----------------|-------------------|------------|
| 1 | Environment & Org Setup | Dev Org, DevHub, Salesforce CLI, VS Code, Project structure | Create Dev Org, enable DevHub, install CLI & extensions, init Git repo | Repo initialized, README with setup steps | Can you create & auth a scratch org via CLI? |
| 2 | Data Model Basics | Objects, Fields, Relationships (Lookup/Master), Standard vs Custom | Create Project & Work Item objects w/ fields; establish relationships | ERD diagram (simple) | Do relationships match use cases? |
| 3 | Advanced Fields | Formula, Roll-Up Summary, Validation Rules, DLRS | 5 validation rules, 3 formulas, 1 roll-up (or DLRS setup) | Documentation of each rule | Do formulas avoid hardcoding IDs? |
| 4 | Security Model | Profiles, Permission Sets, FLS, OWD, Sharing Rules | Configure restricted visibility for Work Items; assign perms via set | Security matrix doc | Can non-admin see only permitted records? |
| 5 | Declarative Automation | Flows vs Process Builder vs Workflow (legacy) | Replace a Workflow with a Record-Triggered Flow | Flow exported image | Is flow bulk-safe & guarded? |
| 6 | Metadata & Deployment | Source tracking, sfdx pull/push, Git branching | Create feature branch, modify metadata, push & merge | Branch + merged PR | Can you rollback via Git? |
| 7 | Review & Mini-Project | Consolidation | Build onboarding process (Flow + validation + sharing) | Demo notes + retrospective | Can you explain each component? |
| 8 | Apex Basics | Syntax, Classes, Methods, Collections | Create Utility class (String/Date helpers) | Apex class + tests | Tests cover >90% lines? |
| 9 | Querying | SOQL, SOSL, Aggregates, Selectivity | Write queries using WHERE, IN, semi-join, aggregate | Query examples md | Do queries use selective filters? |
| 10 | Trigger Framework | One-trigger pattern, Handler class | Implement trigger + handler for Work Item | Trigger + handler + tests | Is trigger bulkified? |
| 11 | Bulkification & Limits | Governor limits, efficient DML | Refactor to handle 200 records in one tx | Updated code + test simulating bulk | No SOQL/DML in loops? |
| 12 | Error Handling | Exceptions, Custom Exceptions | Add custom exception & graceful user message | Exception class + test | Do tests assert thrown exception? |
| 13 | Asynchronous Apex | Future, Queueable, Batch, Scheduled | Implement Queueable to process backlog | Queueable class + test | Can you chain queueables? |
| 14 | Async Continued | Batch Apex patterns, State | Implement Batch for nightly cleanup | Batch class + test | Are batch limits respected? |
| 15 | Integration Basics | Callouts, Named Credentials, Remote Site | Setup Named Credential; simple HTTP callout | Callout class + mock test | Test uses HttpCalloutMock? |
| 16 | Advanced Integration | JSON processing, Custom Settings/Metadata | Parse external JSON, map to objects | Parser util + test | Are nulls handled safely? |
| 17 | Testing Strategy | Test Data Factory, Isolation, SeeAllData=false | Build TestDataFactory & refactor tests | Factory class | Are tests deterministic? |
| 18 | LWC Fundamentals | Component structure, JS/HTML, reactive props | Build basic LWC to list Work Items | LWC bundle + deployed | Does it use @wire correctly? |
| 19 | LWC Data & Wire | @wire Apex, Imperative calls, Caching | Add sorting & imperative refresh | Updated LWC + test (Jest) | Are errors surfaced to user? |
| 20 | LWC UX & Events | Pub/Sub pattern, Custom Events | Parent-child interaction for selection | Event handling code | Are events typed & minimal? |
| 21 | Advanced LWC | LDS (Lightning Data Service), Security | Replace Apex with LDS where possible | Refactored component | Fewer manual SOQL calls? |
| 22 | Packaging & Modules | Namespaces, Folder structure | Reorganize src for clarity; document | Updated repo layout | Clear README architecture? |
| 23 | Performance & Limits | Query optimization, selective indexes | Identify slow queries; add filters | Performance notes | Reduced rows scanned? |
| 24 | Advanced Declarative | Flow error handling, Subflows | Add fault paths & subflow modularization | Flow diagram updates | Fault paths produce clear logs? |
| 25 | Deployment Strategies | Change Sets vs SFDX, Org Differences | Simulated deployment to test scratch org | Deployment script | Can you automate with script? |
| 26 | CI Foundations | GitHub Actions/Shell, sfdx auth | Create simple CI pipeline run tests | YAML workflow file | Pipeline fails on test fail? |
| 27 | Code Quality | PMD, Static Analysis, Formatting | Integrate PMD scan in CI | PMD config + results | Are critical issues resolved? |
| 28 | Advanced Topics | Platform Events, CDC, Pub/Sub | Implement Platform Event & subscriber | Event class + handler | Event triggers testable? |
| 29 | Review & Gap Filling | Revisit weak areas | List gaps & create mini tasks | Gap analysis doc | Are gaps closed? |
| 30 | Capstone & Presentation | End-to-end feature | Build feature: Work Item lifecycle (create, approve, integrate) | Demo script + README | Can you explain design choices? |

## Daily Routine Structure
1. Learn (60–90 min): Trailhead modules / docs
2. Practice (90–120 min): Implement tasks & write tests
3. Review (30 min): Reflect, update README/log
4. Stretch (30 min): Explore related advanced concept

## Tracking Suggestions
- Maintain progress log section (date, tasks, blockers)
- Use GitHub Issues for each day’s deliverables
- Tag commits: day-01, day-02, etc.
- Weekly retrospective: improvements & unresolved questions

## Recommended References
- Trailhead: Apex Specialist, Platform Developer I modules
- Docs: Apex Dev Guide, LWC Dev Guide
- Tools: Salesforce CLI, VS Code Extensions (Apex, SLDS)

## Next Steps After 30 Days
- Prepare for Platform Developer I exam (fill theory gaps)
- Start Platform Developer II superbadges
- Explore advanced integration (Mulesoft, External Services)
