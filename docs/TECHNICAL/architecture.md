# Technical Architecture

## Overview

This document describes the technical architecture of the Sociocultural Project Development Environment.

## Architecture Diagram

The system is designed as an **offline-first, progressive web application (PWA)** with optional desktop and mobile implementations.

### High-Level Architecture

```
Client Layer (PWA/Desktop/Mobile)
├── Presentation Layer (UI Components)
│   ├── User Interface (Vue.js/Svelte)
│   ├── Routing (Vue Router)
│   └── State Management (Pinia)
│
├── Application Layer
│   ├── Services (Data, Sync, Storage, etc.)
│   ├── Utilities (Date, String, File, etc.)
│   ├── Validation (Zod/Yup)
│   └── Internationalization (Vue I18n)
│
└── Data Layer
    ├── Data Access Layer (Repositories)
    ├── Storage Layer (IndexedDB/SQLite)
    └── Sync Manager (Offline-First)

Optional Server Layer (for multi-device sync)
└── Sync Server
    ├── API Gateway
    ├── Authentication Service
    └── Conflict Resolution Service
```

## Component Architecture

### Frontend Structure

```
src/frontend/src/
├── components/
│   ├── common/           # Reusable UI components
│   │   ├── buttons/
│   │   ├── forms/
│   │   ├── modals/
│   │   └── cards/
│   │
│   ├── layout/           # Layout components
│   │   ├── AppHeader.vue
│   │   ├── AppSidebar.vue
│   │   └── PageLayout.vue
│   │
│   └── phases/           # Phase-specific components
│       ├── Phase1Setup/
│       ├── Phase2DataCollection/
│       ├── Phase3Clustering/
│       ├── Phase4Analysis/
│       ├── Phase5Conceptualisation/
│       ├── Phase6Implementation/
│       └── Phase7Evaluation/
│
├── composables/          # Vue composables
├── stores/               # Pinia stores
├── router/               # Vue Router
├── services/             # Business logic services
├── utils/                # Utility functions
└── styles/               # CSS/SCSS
```

### State Management (Pinia)

- `useUserStore()` - User authentication and profile
- `useProjectStore()` - Project management
- `useDataStore()` - Data entries and clustering
- `useAnalysisStore()` - Situation analysis
- `useConceptStore()` - Conceptualisation data
- `useImplementationStore()` - Implementation tracking
- `useEvaluationStore()` - Evaluation data
- `useSyncStore()` - Sync status and queue
- `useUiStore()` - UI state (modals, loading, etc.)

## Data Layer

### Storage Options

| Platform | Storage Technology | Use Case |
|----------|-------------------|----------|
| PWA | IndexedDB (via Dexie) | Primary data storage |
| PWA | OPFS (Origin Private File System) | File storage |
| Desktop | SQLite | Primary data storage |
| Desktop | Local File System | File storage |
| Mobile | SQLite | Primary data storage |
| Mobile | Device Storage | File storage |

### Database Schema

See [Database Schema](database-schema.md) for detailed schema information.

## Offline-First Strategy

### Data Flow

1. **User Action** → UI Component
2. **UI Component** → Service Layer
3. **Service Layer** → Repository (Dexie)
4. **Repository** → IndexedDB/SQLite
5. **Sync Manager** → Queue (if online)
6. **Queue** → Server (optional) or Direct Sync

### Conflict Resolution

- **Timestamp-Based**: Most recent change wins
- **Manual Merge**: Present both versions for user decision
- **Field-Level Merge**: Merge non-conflicting fields automatically
- **Version History**: Keep history of all changes

## Security Architecture

### Data Protection Layers

1. **Application Level**: Input validation, secure coding practices
2. **Storage Level**: Local storage, optional encryption, secure deletion
3. **Data Level**: Data minimization, purpose limitation, storage limitation
4. **User Control**: Consent, export/import, deletion, audit logs

### Encryption Strategy

- **Public Data**: No encryption (project metadata, non-sensitive notes)
- **Sensitive Data**: Optional encryption (personal info, photos with people)
- **Confidential Data**: Always encrypted (passwords, financial info)
- **Implementation**: Web Crypto API (PWA) or Node.js crypto (desktop)
- **Algorithm**: AES-256-GCM

## Accessibility Architecture

### Accessibility Layers

1. **Semantic Foundation**: Semantic HTML5, proper heading hierarchy
2. **ARIA Enhancements**: Roles, properties, labels, live regions
3. **Keyboard Navigation**: Logical tab order, visible focus, shortcuts
4. **Visual Accessibility**: High contrast, large text, colorblind-friendly
5. **Assistive Technology**: Screen reader support, text-to-speech
6. **Cognitive Accessibility**: Clear language, consistent navigation, error prevention

## Performance Architecture

### Optimization Strategies

1. **Data Loading**: Lazy loading, pagination, virtual scrolling
2. **Image Optimization**: Compression (WebP), responsive images, lazy loading
3. **Code Optimization**: Code splitting, tree shaking, minification
4. **Storage Optimization**: Efficient indexing, data compression, cleanup
5. **Memory Management**: Clean up listeners, unmount components, limit cache

## Deployment Options

| Option | Technology | Pros | Cons |
|--------|------------|------|------|
| Static Hosting | GitHub Pages, Netlify, Vercel | Free, easy, HTTPS, CDN | No server features |
| Self-Hosted | Docker, Node.js | Full control, sync server | Maintenance, cost |
| Desktop | Electron, Tauri | Offline, native feel | Larger size, platform-specific |
| Mobile | React Native, Flutter | Native mobile, device features | Platform-specific, approval |
| Offline Distribution | USB, CD/DVD, Local Network | No internet needed | Manual updates |

## Technology Stack

| Category | Recommended | Alternative |
|----------|-------------|-------------|
| Frontend Framework | Vue.js 3 | Svelte |
| State Management | Pinia | - |
| Router | Vue Router | - |
| Database (PWA) | Dexie.js | - |
| Database (Desktop) | SQL.js | - |
| i18n | Vue I18n | - |
| Validation | Zod | Yup |
| Testing (Unit) | Vitest | - |
| Testing (E2E) | Cypress | Playwright |
| Build Tool | Vite | Webpack |

---

*Document Version: 1.0*
*Last Updated: 2024*
