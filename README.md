# 🌱 Eco-Sustain Platform

> **Enhance Eco-Sustain Website** — An integrated civic-tech platform for urban solid waste management, closed-loop recycling logistics, and gamified citizen engagement. Built for the Smart India Hackathon (SIH) prototype.

---

## 📖 Comprehensive Documentation

For the in-depth technical specification, architectural diagrams, data models, entity relationships, and module walkthroughs, please refer to:

👉 **[Complete Technical & Functional Specification (`eco_sustain_documentation.md`)](./eco_sustain_documentation.md)**

### Documentation Quick Links
- **[1. Executive Summary](./eco_sustain_documentation.md#1-executive-summary)**: Problem statement and solutions for duplicate reporting, civic motivation, and disjointed logistics.
- **[2. System Architecture](./eco_sustain_documentation.md#2-system-architecture)**: Client-side architecture diagram, Web Crypto API deduplication, and dynamic in-browser certificate generation.
- **[3. Data Models & Entity Relationships](./eco_sustain_documentation.md#3-data-models--entity-relationships)**: TypeScript entity schemas (`User`, `Certificate`, `Module`, `Event`, `MarketplaceItem`, `Order`, `GarbageType`, `PlantNotification`).
- **[4. Comprehensive Feature Breakdown](./eco_sustain_documentation.md#4-comprehensive-feature-breakdown)**:
  - Role Gateway & Session Switcher
  - Citizen Portal (Dump Reporting, Collection Schedules, Events, Training Certification, Reward Marketplace, Analytics)
  - Green Champion Command Center (Real-time KPIs, Route Optimizer, Waste Dispatch & Plant Notification, Moderation)
  - Processing Plant Portal (Intake View & Load Balancing)
- **[5. Technology Stack & Rationale](./eco_sustain_documentation.md#5-technology-stack--rationale)**: Technical choices (React 18, Vite 6 SWC, Radix UI, shadcn/ui, Tailwind CSS, Motion, Web Crypto API).
- **[6. Directory Structure & Key Files](./eco_sustain_documentation.md#6-directory-structure--key-files)**: Project layout and file organization.
- **[7. Future Enhancement Roadmap](./eco_sustain_documentation.md#7-future-enhancement-roadmap)**: AI waste classification, Leaflet mapping, smart contracts, and backend integration.

---

## 🚀 Key Features Overview

- **Multi-Stakeholder Ecosystem**: Dedicated dashboards tailored for **Citizens**, **Green Champions (Municipal Supervisors)**, and **Processing Plants**.
- **Cryptographic Duplicate Report Prevention**: Uses browser-native Web Crypto API (`SHA-256`) to compute image hashes on upload, filtering out duplicate dump reports without server overhead.
- **Incentivized Citizen Participation**: Earn points through training courses and community drives, redeemable in the marketplace for sustainable goods.
- **Instant Verifiable Eco-Certifications**: Generate and download training completion certificates directly in-browser using the Web Blob API.
- **End-to-End Waste Logistics**: Track municipal zone collection routes, categorize waste streams (Organic, Plastic, Metal), and issue automated dispatches to processing facilities.

---

## 🛠️ Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Framework & Runtime** | [React 18.3](https://react.dev/), [TypeScript 5.3+](https://www.typescriptlang.org/), [Node.js](https://nodejs.org/) |
| **Build Tool** | [Vite 6](https://vitejs.dev/) with `@vitejs/plugin-react-swc` |
| **Styling & UI** | [Tailwind CSS](https://tailwindcss.com/), [Radix UI](https://www.radix-ui.com/), [shadcn/ui](https://ui.shadcn.com/) |
| **Animations** | [Motion](https://motion.dev/) (Framer Motion) |
| **Cryptography** | Native [Web Crypto API (SubtleCrypto)](https://developer.mozilla.org/en-US/docs/Web/API/SubtleCrypto) |
| **Icons & Charts** | [Lucide React](https://lucide.dev/), [Recharts](https://recharts.org/) |
| **Notifications** | [Sonner](https://sonner.emilkowal.ski/) |

---

## 💻 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) (version 18+ recommended) installed on your system.

### Installation

1. Clone or navigate to the repository directory:
   ```bash
   cd SIH2026
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to the local URL displayed in the terminal (typically `http://localhost:5173`).

### Production Build

To build the project for production deployment:
```bash
npm run build
```

---

## 🎨 Design 

- **Figma Design**: [Enhance Eco-Sustain Website on Figma](https://www.figma.com/design/yZjgE04QL4Y1Gc2R5cf0sg/Enhance-Eco-Sustain-Website)
