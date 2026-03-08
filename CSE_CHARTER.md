# Customer Success Engineering Charter

---

## What CSE Is

CSEs are value engineers. We work side-by-side with customer engineers in co-execution sessions, turning ambiguity into clarity and paralysis into action. We don't advise from the sidelines, we don't demo features and hope they stick, and we don't assume the customer understands what Postman Enterprise can actually do for their engineering organization.

We co-execute: build working implementations, prove feasibility and impact in days rather than quarters, and document value objectively upon delivery. Then we hand it off -- to the customer's own team, to Professional Services for paid implementation, or to a TAM for ongoing support.

**Target**: Measurable proof of ROI within 60 days. A value artifact that Sales and leadership can use to power renewal, expansion, and PS pipeline conversations.

---

## Why CSE Exists

**The problem**: Customers buy Postman for user and data governance before understanding the engineering value. They nearly always fail to pivot from PLG value (user-driven behavior -- collections, manual testing, personal workspaces) into the far more impactful and measurable systems of enterprise value that are independent of individual user behavior. When value-per-user is driven by individual behavior, license spend and expansion remain forever under scrutiny.

**The solution**: CSE co-executes with customer engineers to build working, small-scale proof-of-value implementations that embed Postman as infrastructure -- API catalog population, automated contract and smoke testing in CI/CD, governance enforcement, service discovery. This prevents "pilot purgatory" (Gartner: 30%+ of POCs abandoned) by forcing integration, data readiness, and measurable success criteria from day one.

The co-execution model produces 4.1x higher success rates (McKinsey) and is critical for a product like Postman, where the entire value proposition changes between single-user and Enterprise. CSE bridges the gap between what customers think the product does and what it can actually do for their engineering organization at scale.

---

## Why Not [X]?

### Why Not AEs / SEs Alone?

AEs own the commercial relationship and post-sale accountability. SEs own pre-sale technical work and can assist with technical activities that don't require a full CSE engagement. But neither function can dedicate the sustained technical co-execution time that enterprise adoption requires. Credibility matters too: customer engineers engage differently with a fellow engineer who's building alongside them vs someone who's presenting slides.

### Why Not Professional Services?

CSE activates the demand that makes PS viable. Customers rarely pursue large-scale SOW engagements without first experiencing the product through small, surgical implementations. CSE creates internal champions, proves value patterns, and builds the confidence necessary to justify and execute paid professional services. Without that activation layer, PS either stalls on scoping or fails to get the traction necessary to close a contract.

### Why Not TAMs?

TAMs provide ongoing technical support and consultation as paid staff augmentation. In the short term, TAMs and CSEs operate as one team due to capacity constraints. As the function scales, TAMs will transition to accounts that pay for ongoing augmentation. CSE focuses on the initial high-intensity engagement: prove value, build the pattern, hand off. TAMs maintain and extend.

---

## The CSE Motion: Platform Integration

The core CSE engagement follows a consistent pattern regardless of the customer's specific stack:

**Discover** -- Identify what's deployed (via API gateway integration, Insights agent, or repo scanning). Understand the customer's infrastructure: SCM, CI/CD, cloud provider, auth patterns, deployment topology.

**Onboard** -- Ingest API specs into Spec Hub. Generate collections (baseline, contract, smoke). Configure environments. Link workspaces to repos. Populate the API catalog so services are discoverable in seconds instead of hours.

**Automate** -- Install CI/CD pipelines that run contract and smoke tests on every deploy. Set up monitors for continuous drift detection. Wire governance rules so spec quality is enforced before merge.

**Prove** -- Show measurable results: discovery time reduced from hours to seconds, test coverage from 0% to automated baselines, API health visible in one place for the first time. Quantify ROI for the executive audience.

**Hand off** -- Transfer the pattern to the customer's platform/ops team. Leave behind documented workflows, parameterized templates, and a self-serve path for onboarding new services. CSE exits; PS or TAM picks up if the customer wants ongoing support.

---

## Success Sprints

| Sprint | What It Is | CSE Delivers |
|--------|-----------|--------------|
| **API Catalog & Service Discovery** | Populate the API catalog from existing infrastructure (gateway discovery, Insights agent, spec ingestion). Make every API discoverable and documented in Postman. | Working catalog with service inventory, <30 sec discoverability, dependency mapping where available |
| **Asset Ingestion & Dev Systems Integration** | Corral scattered APIs into governed workspaces, connect to Git repos, link specs to collections, tie into existing dev tools | Pipeline for systemic API asset ingestion, workspace rationalization, reduced time-to-first-call |
| **Testing Maturation** | Activate automated contract and smoke testing in the customer's CI/CD pipeline | Working CI/CD example with generated tests, coverage visibility across services, monitoring for spec drift |
| **Governance Maturation** | Establish spec-first development and controlled change | Spec linting in CI, governance rules enforced before merge, style guides, workspace access controls |
| **Agent Mode & AI Adoption** | Systematize AI-assisted development patterns using the populated API catalog as the knowledge base | Agent Mode queries across the full catalog, MCP server workflows, AI-generated test suites, semantic insights on API health |

---

## Core Plays

| Play | When | CSE Delivers |
|------|------|--------------|
| **Discovery / Intelligence Gathering** | Before any engagement. Research the customer's public API surface, Postman asset quality, and software development posture. | Findings document, recommended engagement scope, success plan guidance |
| **Reverse Demo** | Early engagement. Customer demos their current state; CSE maps the landscape and proposes a reality-grounded future state. | Working reference implementation, gap-to-target mapping |
| **Proof of Value** | Core engagement. Propose solution based on discovery, build it at small scale, prove feasibility with the customer's actual infrastructure. | Working implementation the customer can replicate or use to justify additional license/services spend |
| **Ad-Hoc Solutioning** | As needed. Unblock adoption barriers that appear unsolvable with known product functions. | Working solution or workaround; documented pattern for future reference |
| **Product Feedback Loop** | Continuous. Filter through blockers to determine what is/isn't a product gap and provide tailored input to product teams. | Validated gap assessment with business value context; prioritized input to PM roadmap |

---

## Core Artifacts

| Artifact | Purpose |
|----------|---------|
| **Build Logs** | Structured documentation of POV delivery: what was built, how long it took, what value was unlocked. Arms the team for impact reviews and provides evidence against procurement-driven churn. |
| **Reusable Templates & Actions** | Pre-built GitHub Actions, workflow templates, CI/CD configs, demo environments, and spec ingestion tooling that accelerate future POVs. |
| **Success Narratives** | Customer-validated stories documenting the before/after: problem, solution, measurable outcome. Used for internal case studies and executive briefings. |

---

## How to Engage CSE

**Default**: All incoming accounts over $250K will have a CSE assigned where capacity allows. AEs supporting these accounts can request post-sale technical support through the intake portal.

For accounts under $250K, SEs provide technical support as needed. CSE engagement requires a specific justification.

**What Qualifies for CSE**

Engage CSE when all of these are true:

1. The goal is technical adoption -- not SSO setup, not onboarding, not break/fix
2. A named technical lead on the customer side has dev systems access and will co-work with the CSE
3. There's a clear desire for transformation (not just "help us use Postman more")
4. The scope fits a success sprint or play above

**Standard Triggers:**

- IT foundation exists (SSO, licensing, basic setup done), but engineering value does not
- Workspace sprawl causing low trust and poor discoverability
- Renewal risk with no measurable success evidence
- V12 upgrade opportunity with platform integration potential
- Expansion opportunity requiring new use case activation

**The Bright Line**: No goal, no acceptance criteria, no customer engineer to work with = not a CSE engagement.
