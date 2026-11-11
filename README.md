<p align="center">
  <img src="https://raw.githubusercontent.com/wondxpt/Xperslot-Showcase/main/xperslot-banner.svg" width="100%" alt="XperSlot — Scheduling that works as one connected system." />
</p>

<h1 align="center">XperSlot</h1>
<p align="center"><strong>Service booking and business operations, delivered through two dedicated apps.</strong></p>

<p align="center">
  <img alt="Product stage" src="https://img.shields.io/badge/Stage-Android%20Preview%20Validation-0F766E?style=for-the-badge" />
  <img alt="Apps" src="https://img.shields.io/badge/Apps-Customer%20%2B%20Business-164E63?style=for-the-badge" />
  <img alt="Platforms" src="https://img.shields.io/badge/Platforms-Web%20%2B%20Android-5A55E0?style=for-the-badge" />
  <img alt="Application source" src="https://img.shields.io/badge/Application%20Source-Private-475569?style=for-the-badge" />
</p>

XperSlot is an independently developed SaaS product for service discovery, appointment booking, and business operations. Its current product structure consists of **two separate applications** connected through shared account, booking, and business services—not a single role-switching app.

**Official links:** [Android release hub](https://github.com/wondxpt/XperSlot-Downloads) · [Developer profile](https://github.com/wondxpt)

## The two apps

<table>
  <tr>
    <td width="50%" valign="top">
      <h2>XperSlot Customer</h2>
      <p><strong>Discover, compare, and book.</strong></p>
      <ul>
        <li>Discover service businesses and professionals.</li>
        <li>Explore categories, services, profiles, portfolios, and reviews.</li>
        <li>Book appointments and manage upcoming or past bookings.</li>
        <li>Save favourites and contact providers.</li>
        <li>Manage a personal profile and customer journey.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h2>XperSlot Business</h2>
      <p><strong>Run the day-to-day business workspace.</strong></p>
      <ul>
        <li>Configure business details, services, and availability.</li>
        <li>Manage calendars, appointments, and waitlists.</li>
        <li>Organise team members, shifts, resources, and time off.</li>
        <li>Maintain client records and customer communication.</li>
        <li>Access operational tools such as checkout, inventory, reviews, loyalty, and reporting where enabled.</li>
      </ul>
    </td>
  </tr>
</table>

Feature availability depends on account permissions, workspace configuration, and connected services. The feature lists describe product scope; they are not a claim that every capability is generally available in production.

## Why two apps?

Customers and service businesses have different goals and information needs. XperSlot separates the customer discovery-and-booking journey from the business workspace while connecting both through shared booking and account services. Each app can stay focused on the tasks of its audience without forcing both groups into a role-switching interface.

## Conceptual architecture

<p align="center">
  <img src="https://raw.githubusercontent.com/wondxpt/Xperslot-Showcase/main/architecture.svg" width="100%" alt="Conceptual XperSlot architecture: separate customer and business experiences connect through application APIs to booking, client, messaging, integration, identity, and data services." />
</p>

The diagram explains product boundaries and responsibilities at a high level. It is **not** a deployment topology, a complete security design, or proof that every integration is enabled in production.

## Engineering focus

- **Multi-tenant access:** validate workspace membership and permissions at the API and data layers.
- **Scheduling correctness:** preserve service duration, staff availability, and appointment state through booking workflows.
- **Communication flows:** connect customer conversations and team communication to the correct records and permissions.
- **Cross-platform UX:** maintain coherent web and Android behavior, including localization and right-to-left layouts.
- **Operational reliability:** make failures observable and validate journeys across the interface, API, and persistence layers.

## Technology

<p>
  <img alt="React" src="https://img.shields.io/badge/React-149eca?style=flat-square&logo=react&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img alt="Supabase" src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=1A1A1A" />
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img alt="Vite" src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
  <img alt="Capacitor" src="https://img.shields.io/badge/Capacitor-119EFF?style=flat-square&logo=capacitor&logoColor=white" />
  <img alt="Android" src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=1A1A1A" />
</p>

## Android release status

**11 November 2026 — Preview validation in progress.** Local Customer and Business release APKs have verified package metadata, SHA-256 checksums, and APK Signature Scheme v2 signatures. A GitHub prerelease draft is being prepared, but its APK assets are not yet confirmed as fully uploaded. **There are no public APK downloads at this time.**

The current candidates are Customer 2.1 (code 13) and Business 2.9.4 (code 27). They are signed with a release certificate that differs from the certificate on certain earlier test installations. Android will reject an in-place update from those installations. Do not uninstall existing apps or treat these candidates as compatible updates.

See the [release status and verification record](https://github.com/wondxpt/XperSlot-Downloads/blob/main/RELEASE_STATUS.md) and [published releases](https://github.com/wondxpt/XperSlot-Downloads/releases). Only a release with both completed APK attachments is a public download.

## About the maker

Built by [Abbas Shiri](https://github.com/wondxpt), a developer focused on web and mobile products, SaaS architecture, and end-to-end workflows.

Also see [ResuMetrics](https://github.com/wondxpt/ResuMetrics), a separate resume and CV builder project.

---

<p align="center"><sub>XperSlot · Product overview · Proprietary application source maintained privately</sub></p>
