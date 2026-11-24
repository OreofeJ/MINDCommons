# MINDCommons
###  What if communities can exercise agency over responsible use of sensitive health data?
###  Can Community centred health data governance and privacy infrastructure be a collective responsibly?

MINDCommons is an initiative exploring how communities can exercise meaningful agency over the collection, access, governance and responsible use of sensitive health data, particularly in underserved African contexts.

The project focuses on developing practical, transparent and reusable digital infrastructure that supports individual consent, accountable data access and community-centred governance.

Rather than treating data protection as solely a technical or institutional responsibility, MINDCommons explores how privacy infrastructure can support stronger relationships between stakeholders such as individuals, communities, researchers and health institutions.

## The vision

Health data can support research and public health innovation . However, its use must be accompanied by meaningful consent and accountable access mechanisms. It must also be supported by governance arrangements that respect the interests of the people and communities represented in that data.

MINDCommons explores a complementary approach built around two foundational capabilities:

1. **Individual consent management:** enabling individuals to register, manage and withdraw consent for specific data-use purposes.
2. **Governed data access:** providing mechanisms to evaluate research access requests against consent requirements and applicable governance policies, with traceable decisions.

## Technical architecture

The initial technical portfolio consists of two complementary MVPs.

### 1. HDC: Health Data Consent
<img width="1416" height="1860" alt="HDC" src="https://github.com/user-attachments/assets/7e1d4568-9f8d-4820-ab20-84612cf65270" />

[Explore HDC](./projects/hdc/)

HDC is a consent management and verification prototype focused on individual, purpose-specific consent.

Its initial capabilities include:

- Consent registration and management.
- Consent withdrawal.
- Consent-status verification.
- Consent-purpose tracking.
- Audit-trail visibility.

**Current status:** Early-stage frontend system. 

### 2. DataTrust Gate: Health Data Access Governance
<img width="1892" height="861" alt="dtg" src="https://github.com/user-attachments/assets/8218c750-2918-4e1e-9938-c414099f34dd" />

[Explore DataTrust Gate](./projects/datatrust-gate/)

DataTrust Gate is a prototype for community-governed health-data access control and auditing in Nigeria.

Its capabilities include:

- Researcher access-request management.
- Governance-policy configuration.
- Deterministic access-decision evaluation.
- Approved, Denied and Review outcomes.
- Consent-reference verification workflows.
- Audit-event recording.
- Dashboard-based governance monitoring.

**Current status:** Deployed system using a React and TypeScript frontend, Node.js backend and Firebase Firestore persistence.

DataTrust Gate is designed to complement HDC rather than duplicate its consent-management responsibilities. Integration between the two systems is a planned development milestone.

An approval decision does not itself authorise unrestricted access to, or transfer of, underlying health data.

## Supporting research

### Predicting Pathogen Emergence Using a Spatiotemporal Graph Neural Network and Explainable AI Approach

[Explore the research materials](./research/pathogen-emergence-paper/)

This research examines the application of spatiotemporal graph learning and explainable AI to pathogen emergence prediction.

It represents complementary research experience in machine learning, public health and responsible AI. It is included as supporting research rather than as a component of the MINDCommons software architecture.

**Status:** Research paper submitted for publication.

## How the components relate

The intended relationship between the two technical systems is:

- **HDC** manages individual consent and exposes consent-verification capabilities.
- **DataTrust Gate** evaluates researcher access requests against applicable governance policies and consent requirements.
- **MINDCommons** provides the broader conceptual framework for connecting individual agency, accountable access and community-centred health-data governance.

The planned integration will allow DataTrust Gate to verify consent through HDC's API rather than relying on synthetic consent references.

## Repository structure

```text
MINDCommons/
├── README.md
├── projects/
│   ├── hdc/
│   │   └── HDC application
│   └── datatrust-gate/
│       └── DataTrust Gate application
└── research/
    └── pathogen-emergence-paper/
        └── Research paper and supporting materials
```

## Development roadmap

| Milestone | Focus | Status |
|---|---|---|
| v0.1 | HDC consent-management MVP | Built |
| v0.1 | DataTrust Gate access-governance MVP | Built and deployed |
| v0.2 | Persistent HDC backend and API | Planned |
| v0.2 | HDC–DataTrust Gate integration | Planned |
| Future | Expanded governance and community-review workflows | Under consideration |

## Responsible development and limitations

MINDCommons is under active development. The current prototypes demonstrate technical approaches and early implementation capabilities; they should not be interpreted as evidence of a fully operational community-governance system.

## Technology

The current portfolio uses:

- React and TypeScript
- Tailwind CSS
- Node.js
- Firebase Firestore
- Google Cloud Run
- GitHub

The technology choices may evolve as the architecture develops.

## Contributing and collaboration

MINDCommons is an evolving research and technical initiative. Collaboration with researchers, public-health practitioners, community organisations, data-governance specialists and responsible-AI practitioners is welcome.

## Contact

For research collaboration, technical discussions or partnership enquiries, please use the contact information associated with this GitHub profile.

---

**MINDCommons is working towards community centred and responsible health data governance.**
