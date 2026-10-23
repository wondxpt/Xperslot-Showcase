<p align="center">
  <img src="https://raw.githubusercontent.com/wondxpt/Xperslot-Showcase/main/xperslot-banner.svg" width="100%" alt="Xperslot — Scheduling that works as one connected system" />
</p>

<p align="center">
  <strong>A multi-tenant booking and business-operations platform designed around two clear experiences: Business and Customer.</strong>
</p>

<p align="center">
  <img alt="Product stage" src="https://img.shields.io/badge/Stage-Preparing%20for%20Release-0F766E?style=for-the-badge" />
  <img alt="Launch status" src="https://img.shields.io/badge/Public%20Launch-Coming%20Soon-5A55E0?style=for-the-badge" />
  <img alt="Web and mobile" src="https://img.shields.io/badge/Platforms-Web%20%2B%20Android-164E63?style=for-the-badge" />
  <img alt="Source" src="https://img.shields.io/badge/Application%20Source-Private-475569?style=for-the-badge" />
</p>

Xperslot is an independently developed SaaS product focused on bringing online booking and day-to-day business workflows into one connected system. The product is being built with separate customer-facing and business-facing experiences, backed by shared services and tenant-aware access rules.

> **Release update:** Xperslot is being finalized and prepared for public release. **Public launch coming soon.** This repository presents the product direction and architecture; proprietary application source remains private.

## Product direction

Xperslot is designed to make the full journey easier to manage—from finding a service and choosing an available time to running the schedule and maintaining customer relationships.

| Customer experience | Business experience |
| --- | --- |
| Discover businesses and services | Configure services, staff, and availability |
| Explore available appointment times | View and manage the booking calendar |
| Create and manage bookings | Maintain client and booking information |
| Keep communication connected to the booking journey | Handle client conversations and team communication |
| See a clear experience across devices | Coordinate daily work in a dedicated workspace |

The two experiences are separate product surfaces rather than a single interface with a role switch.

## Engineering focus

The product work emphasizes complete, testable workflows—not just static screens.

- **Multi-tenant boundaries:** isolate business data and verify membership and permissions at the API and data layers.
- **Scheduling correctness:** keep service duration, staff availability, and appointment changes consistent through booking workflows.
- **Communication flows:** connect client conversations and internal team communication to the appropriate permissions and records.
- **Calendar integrations:** support an explicit authorization flow and keep external calendar events aligned with booking changes.
- **Cross-platform UX:** keep web and mobile interactions coherent, including localization and right-to-left layouts where needed.
- **Operational reliability:** make errors observable and validate user journeys across the interface, API, and persistence layers.

## High-level architecture

<p align="center">
  <img src="https://raw.githubusercontent.com/wondxpt/Xperslot-Showcase/main/architecture.svg" width="100%" alt="Conceptual Xperslot product architecture diagram" />
</p>

The diagram is intentionally high-level. It illustrates product boundaries and core responsibilities; it is not a deployment map, a complete threat model, or a promise that every capability is generally available today.

## Technology

<p>
  <img alt="React" src="https://img.shields.io/badge/React-149eca?style=flat-square&logo=react&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img alt="Supabase" src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=1A1A1A" />
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img alt="Vite" src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
  <img alt="Android" src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=1A1A1A" />
  <img alt="OAuth" src="https://img.shields.io/badge/OAuth-18181B?style=flat-square&logo=openid&logoColor=white" />
</p>

The stack supports a typed web client, a Node.js API, managed authentication and PostgreSQL data services, and a mobile delivery path. Exact implementation details and security-sensitive configuration remain in the private application repository.

## Release status

Xperslot is being completed and prepared for public release. The public launch is coming soon. This overview describes the product direction and architecture; availability of individual features may vary as release preparation continues.

## About the maker

Built by [Abbas Shiri](https://github.com/wondxpt), a full-stack developer focused on web and mobile products, SaaS architecture, and end-to-end workflows.

Also see [ResuMetrics](https://github.com/wondxpt/ResuMetrics), a separate resume/CV builder project.

---

<p align="center"><sub>Xperslot · Product overview · Proprietary source maintained privately</sub></p>
