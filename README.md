<img width="1536" height="1024" alt="overview" src="https://github.com/user-attachments/assets/4e782d72-ccd0-415e-b31b-c6b4a4d7ed37" />


# Velora

### The operating platform for modern photographers.

Velora is a photography-first platform designed to help photographers build their online presence, showcase their work, manage galleries, handle bookings, understand their audience, and operate their photography business from one place.

> **Status:** Version 1 — In Development
> **Repository:** Proprietary / Private Intellectual Property
> **Owner:** Patrick Obialor / Velora

---

## Overview

Velora is being built as a modern alternative to fragmented photography business tools.

Instead of forcing photographers to combine a portfolio website, online gallery service, booking tools, client management, and analytics from different products, Velora is designed around a unified photography-first experience.

The product philosophy is simple:

**Beautiful work deserves beautiful infrastructure.**

Velora prioritizes:

* Photography-first presentation
* Elegant and minimal interfaces
* Fast interactions
* Simple workflows
* Professional client experiences
* Gallery management
* Booking management
* Business analytics
* Scalable workspace infrastructure

---

# Product

Velora V1 is being developed around the following core areas:

```text
Velora
│
├── Marketing Website
│
├── Authentication
│   ├── Register
│   ├── Login
│   └── Password Recovery
│
├── Onboarding
│
└── Photographer Dashboard
    ├── Overview
    ├── Galleries
    ├── Bookings
    ├── Clients
    ├── Analytics
    └── Settings
```

Additional capabilities may be introduced in future versions.

---

# Design Philosophy

Velora is intentionally not designed as a generic SaaS administration panel.

The interface follows a photography-first visual language combining:

* Editorial composition
* Spacious layouts
* Restrained color usage
* Strong typography
* Large visual surfaces
* Subtle interaction feedback
* Minimal interface noise
* Premium but approachable presentation

### Color Distribution

Velora follows an approximate:

```text
85% — Neutral
10% — Brand
5%  — Feedback / Status
```

The primary brand color is Velora forest green.

```css
--velora-green: #1b4332;
--velora-green-dark: #123325;
--velora-green-tint: #e9f0ec;
```

---

# Design System

Velora uses a token-first design system.

The architecture follows:

```text
Brand Palette
      ↓
Primitive Tokens
      ↓
Semantic Tokens
      ↓
Component Tokens
      ↓
Components
      ↓
Pages
```

Reusable design values should come from approved design tokens rather than arbitrary hard-coded values.

### Core Tokens

```css
--velora-ink: #17181a;
--velora-paper: #ffffff;
--velora-line: #ececec;
--velora-muted: #63676c;

--velora-green: #1b4332;
--velora-green-dark: #123325;
--velora-green-tint: #e9f0ec;
```

---

# Frontend Architecture

The frontend follows a structured CSS architecture:

```text
css/
│
├── tokens/
│   ├── colors.css
│   ├── typography.css
│   ├── spacing.css
│   ├── radius.css
│   ├── shadows.css
│   ├── motion.css
│   ├── breakpoints.css
│   └── z-index.css
│
├── base/
│
├── utilities/
│
├── layout/
│
├── components/
│
├── pages/
│
└── vendors/
```

Reusable components use the `velora-` prefix.

Design-system utility classes use the `v-` prefix.

Examples:

```text
velora-navbar
velora-card
velora-dashboard
velora-gallery
```

and:

```text
v-text-h1
v-mt-4
v-flex
```

---

# Component Standards

Every approved Velora component is expected to have:

* Unique component ID
* Defined lifecycle status
* Defined maturity level
* Documented design decisions
* Responsive behavior
* Accessibility considerations
* Interaction states
* Testing requirements
* Implementation documentation

### Component Lifecycle

```text
Draft
  ↓
Under Review
  ↓
Approved
  ↓
Deprecated
  ↓
Archived
```

### Maturity Levels

```text
L1 — Experimental
L2 — Stable
L3 — Core
L4 — Platform
```

A component should not enter the official Velora component library unless it meets the project's **9.5/10 quality standard**.

---

# Documentation Before Implementation

Velora follows a strict:

> **Documentation Before Implementation**

workflow.

The intended process is:

```text
Idea
 ↓
Documentation
 ↓
Design Decision
 ↓
Review
 ↓
Component ID
 ↓
Implementation
 ↓
Testing
 ↓
Quality Review
 ↓
Approval
```

No major feature or reusable component should be implemented without first establishing its intended role and architecture.

---

# Current V1 Progress

### Marketing Website

* [x] Navigation
* [x] Hero
* [x] Template showcase
* [x] Everything Your Photography Needs
* [x] Product workflow section
* [x] Feature sections
* [x] Pricing
* [x] FAQ
* [x] Footer
* [x] Responsive refinement

### Authentication

* [x] Registration UI
* [x] Login UI
* [x] Forgot Password UI
* [x] Authentication responsive states

### Onboarding

* [x] Workspace setup
* [x] Photography category selection
* [x] Workspace URL setup
* [x] Progress navigation
* [x] Responsive layout

### Dashboard

* [x] Dashboard shell
* [x] Sidebar navigation
* [x] Top navigation
* [x] Mobile navigation
* [ ] Overview
* [ ] Galleries
* [ ] Bookings
* [ ] Clients
* [ ] Analytics
* [ ] Settings

---

# Technology

The current frontend foundation includes:

* HTML5
* CSS3
* Bootstrap 5
* Bootstrap Icons
* JavaScript
* Lato
* Responsive CSS architecture

The technology stack may evolve as Velora moves from prototype to production.

---

# Repository Structure

The repository is organized around separation of concerns.

```text
velora/
│
├── index.html
│
├── register.html
├── login.html
├── forgot-password.html
├── onboarding.html
├── dashboard.html
│
├── css/
│   ├── style.css
│   ├── register.css
│   ├── login.css
│   ├── forgot-password.css
│   ├── onboarding.css
│   └── dashboard.css
│
├── media/
│   ├── logo/
│   ├── favicon/
│   ├── banner/
│   └── dashboard/
│
├── docs/
│
└── README.md
```

---

# Intellectual Property & Copyright

© 2026 Patrick Obialor. All rights reserved.

**Velora, its branding, product concepts, visual identity, design system, interface designs, source code, documentation, architecture, graphics, copy, workflows, and other original materials contained in this repository are proprietary intellectual property of the project owner, except where otherwise stated.**

This repository is **not an open-source project**.

Unless explicit written permission has been granted by the owner, you may not:

* Copy the source code
* Reproduce the interface
* Republish the project
* Redistribute the repository
* Sell or sublicense the software
* Repackage the source code
* Create a derivative commercial product
* Reuse Velora's proprietary design system
* Reuse Velora's branding or visual identity
* Present Velora's work as your own
* Use substantial portions of this repository in another product
* Publish screenshots, designs, or proprietary documentation for commercial purposes

Viewing this repository does **not** grant ownership, licensing rights, redistribution rights, or commercial usage rights.

Any third-party libraries, frameworks, fonts, icons, images, or other assets remain subject to their respective licenses and ownership terms.

---

# Proprietary License

Permission is granted to authorized contributors to access and modify this repository solely for the purpose of developing Velora.

No permission is granted to third parties to reproduce, distribute, sublicense, sell, or commercially exploit this software or its proprietary assets without prior written authorization.

Unauthorized copying, reproduction, redistribution, or commercial exploitation of proprietary materials may constitute infringement of applicable intellectual property rights.

For licensing, partnership, contribution, or commercial-use inquiries, contact the project owner before using proprietary materials.

---

# Ownership Notice

The presence of this repository on GitHub does not transfer ownership of any intellectual property contained within it.

GitHub provides repository hosting and version-control infrastructure; it does not establish ownership of the project's underlying intellectual property.

All original Velora materials remain owned by their respective rights holders.

Where ownership has been assigned to or is held by the project owner, that ownership remains with the project owner unless transferred through a separate written agreement.

---

# Contributions

Velora is currently developed as a proprietary project.

External contributions are not automatically accepted.

Any contribution, suggestion, code submission, design, documentation, or other material submitted to the project may be subject to separate contribution terms established by the project owner.

Do not submit confidential or third-party proprietary material.

---

# Third-Party Materials

This repository may contain dependencies or assets owned by third parties.

Examples may include:

* Bootstrap
* Bootstrap Icons
* Google Fonts
* Other open-source libraries
* Licensed photography
* Third-party services

Those materials are **not claimed as Velora-owned intellectual property**.

Their respective licenses continue to apply.

---

# Security

Do not commit:

* API keys
* Passwords
* Authentication secrets
* Database credentials
* Private tokens
* Production environment variables
* Private customer information

Use environment variables and appropriate secret-management infrastructure when production integrations are introduced.

Security vulnerabilities should be reported privately rather than publicly exposing exploitable details.

---

# Development Principle

Velora is being developed with a long-term product mindset.

The goal is not simply to create another portfolio website.

The goal is to build infrastructure that allows photographers to present their work, manage their clients, operate their business, and grow their digital presence from one coherent platform.

```text
Beautiful work
       +
Simple infrastructure
       +
Professional experience
       ↓
     VELORA
```

---

# Project Status

**Velora V1 is currently under active development.**

Features, architecture, interfaces, pricing, technology, and product decisions may change as the product progresses.

The documentation in this repository should be treated as a living record of the project's current architecture and development direction.

---

# Copyright

```text
Copyright © 2026 Patrick Obialor.
All rights reserved.

Velora is proprietary software.

Unauthorized reproduction, distribution,
commercial use, or derivative works are prohibited
unless expressly authorized in writing by the owner.
```

**Velora — Built for photographers.**
