# Modern Laravel Frontend Ecosystem Roadmap
### Zero to Senior Laravel + Vue.js Full Stack Developer

> **Last reviewed:** July 2026, against the current stable Vue/Tailwind/Pinia ecosystem. Updated for: Tailwind v4 CSS-first config, Pinia Colada, Storybook, frontend observability, typed OpenAPI clients, and Vapor Mode awareness. See the study-order note before Phase 4 for a TypeScript-earlier recommendation.

---

# Phase 1 - JavaScript Essentials

- [ ] Variables (var, let, const)
- [ ] Data Types
- [ ] Type Coercion
- [ ] Operators
- [ ] Template Literals
- [ ] Conditionals
- [ ] Loops (for, for...of, for...in, while)
- [ ] Functions
- [ ] Arrow Functions
- [ ] Default Parameters
- [ ] Rest Parameters
- [ ] Spread Operator
- [ ] Destructuring (Objects & Arrays)
- [ ] Array Methods (map, filter, reduce, find, some, every, forEach, sort, includes)
- [ ] Object Methods (keys, values, entries, assign, freeze)
- [ ] Optional Chaining
- [ ] Nullish Coalescing
- [ ] Scope & Hoisting
- [ ] Closures
- [ ] `this` Keyword
- [ ] Call, Apply, Bind
- [ ] Prototypes & Prototypal Inheritance
- [ ] Classes
- [ ] Getters & Setters
- [ ] Static Methods & Properties
- [ ] Modules (import/export)
- [ ] Promises
- [ ] Async/Await
- [ ] Fetch API
- [ ] Error Handling (try/catch)
- [ ] Event Loop
- [ ] Microtasks vs Macrotasks
- [ ] JSON (parse/stringify)
- [ ] DOM Basics
- [ ] Event Handling Basics
- [ ] LocalStorage / SessionStorage
- [ ] Sets & Maps
- [ ] Symbols
- [ ] Generators & Iterators
- [ ] Debounce & Throttle Concepts
- [ ] Immutability Concepts
- [ ] Shallow vs Deep Copy

---

# Phase 2 - Vue.js Fundamentals

- [ ] Vue Architecture Overview
- [ ] Reactivity Internals (Proxies, Dependency Tracking, Effect Scheduling) — *the concept behind ref/reactive, taught here so it's not a last-minute interview cram*
- [ ] Vue Project Structure
- [ ] Vue CLI Basics
- [ ] Vite Basics
- [ ] Creating a Vue App
- [ ] Single File Components (SFC)
- [ ] Template Syntax
- [ ] Interpolation
- [ ] Directives (v-bind, v-model, v-if, v-else, v-else-if, v-show, v-for, v-on, v-slot, v-html, v-pre, v-once, v-cloak)
- [ ] Reactivity Fundamentals
- [ ] ref()
- [ ] reactive()
- [ ] Reactive Objects vs Refs
- [ ] Computed Properties
- [ ] Watch
- [ ] WatchEffect
- [ ] Lifecycle Hooks (all)
- [ ] Event Handling
- [ ] Form Input Bindings
- [ ] v-model Modifiers
- [ ] Conditional Rendering
- [ ] List Rendering
- [ ] Key Attribute Importance
- [ ] Components Basics
- [ ] Component Registration (Global & Local)
- [ ] Props
- [ ] Props Validation
- [ ] Emits
- [ ] Custom Events
- [ ] Slots
- [ ] Named Slots
- [ ] Scoped Slots
- [ ] Dynamic Components
- [ ] Async Components
- [ ] KeepAlive
- [ ] Teleport
- [ ] Suspense
- [ ] Provide / Inject
- [ ] Custom Directives
- [ ] Plugins
- [ ] Mixins
- [ ] Composables Basics
- [ ] Render Functions
- [ ] JSX Basics in Vue
- [ ] Template Refs
- [ ] Fragment Support
- [ ] Global Properties
- [ ] Attribute Inheritance
- [ ] Fallthrough Attributes

---

# Phase 3 - Composition API (Deep Dive)

- [ ] Options API vs Composition API
- [ ] *(Legacy Awareness)* Reading & Maintaining Options API Code — not for new projects, but needed to work in older/legacy codebases
- [ ] setup() Function
- [ ] `<script setup>` Syntax
- [ ] Reactive State Management
- [ ] Computed in Composition API
- [ ] Watchers in Composition API
- [ ] Lifecycle Hooks in Composition API
- [ ] Composables Design Patterns
- [ ] Reusable Logic Extraction
- [ ] Dependency Injection with provide/inject
- [ ] toRef & toRefs
- [ ] unref
- [ ] isRef, isReactive, isProxy
- [ ] readonly()
- [ ] shallowRef & shallowReactive
- [ ] markRaw
- [ ] customRef
- [ ] effectScope
- [ ] Template Refs in Composition API
- [ ] Composition API with TypeScript Basics
- [ ] Organizing Large Components with Composables
- [ ] Testing Composables

---

> **Study-order note:** Before continuing to Phase 4, skim the "TypeScript Basics for Vue" section of Phase 17 (Typing Props, Typing Refs, Type Inference in `<script setup>`) as a lightweight primer. You'll be typing Router params, Pinia stores, and Axios responses from here on — better to know the basics now than retrofit types later. Come back to Phase 17 in full for the deep dive.

# Phase 4 - Vue Router

- [ ] Router Installation & Setup
- [ ] Route Definitions
- [ ] Named Routes
- [ ] Dynamic Routes
- [ ] Nested Routes
- [ ] Route Params
- [ ] Query Params
- [ ] Programmatic Navigation
- [ ] Router-Link Component
- [ ] Router-View Component
- [ ] Navigation Guards (Global, Per-Route, In-Component)
- [ ] beforeEach, beforeResolve, afterEach
- [ ] Route Meta Fields
- [ ] Protected Routes / Auth Guards
- [ ] Lazy Loading Routes
- [ ] Route-Based Code Splitting
- [ ] Scroll Behavior
- [ ] Redirect & Alias
- [ ] History Mode vs Hash Mode
- [ ] 404 / Catch-All Routes
- [ ] Route Transitions
- [ ] Composable-Based Route Access (useRoute, useRouter)
- [ ] Advanced Router Patterns
- [ ] Router Testing

---

# Phase 5 - Pinia (State Management)

- [ ] Why Pinia over Vuex
- [ ] Store Setup
- [ ] Defining Stores (Options Style)
- [ ] Defining Stores (Setup Style)
- [ ] State
- [ ] Getters
- [ ] Actions
- [ ] Using Stores in Components
- [ ] Store Composition (Using One Store in Another)
- [ ] Store Reset
- [ ] Store Subscriptions
- [ ] Plugins in Pinia
- [ ] Persisted State
- [ ] Devtools Integration
- [ ] Modular Store Architecture
- [ ] Testing Pinia Stores
- [ ] Pinia with TypeScript
- [ ] Pinia Colada Awareness — the official async/server-state companion to Pinia (caching, dedup, background revalidation); compare against TanStack Query in Phase 19 when you get there

---

# Phase 6 - Axios & API Integration

- [ ] Axios Installation & Configuration
- [ ] Base URL & Instances
- [ ] GET, POST, PUT, PATCH, DELETE Requests
- [ ] Request & Response Interceptors
- [ ] Headers Configuration
- [ ] Error Handling Strategies
- [ ] Global Error Handling
- [ ] Loading States
- [ ] Cancel Tokens / AbortController
- [ ] Request Retrying
- [ ] File Uploads with Axios
- [ ] Progress Tracking
- [ ] Authentication Tokens (Bearer)
- [ ] Refresh Token Handling
- [ ] Centralized API Service Layer
- [ ] Environment-Based API Configuration

---

# Phase 7 - Forms

- [ ] Form Binding Basics
- [ ] Controlled vs Uncontrolled Inputs
- [ ] Form Validation Basics
- [ ] Client-Side Validation Libraries
- [ ] Custom Validation Rules
- [ ] Error Message Handling
- [ ] Displaying Backend Validation Errors
- [ ] Multi-Step Forms
- [ ] Dynamic Form Fields
- [ ] File Uploads
- [ ] Multipart Form Data
- [ ] Image Preview Before Upload
- [ ] Reusable Form Components
- [ ] Form State Management
- [ ] Debounced Input Validation
- [ ] Form Reset & Dirty State Tracking
- [ ] Accessibility in Forms

---

# Phase 8 - CRUD Applications

- [ ] Listing Data (Index Pages)
- [ ] Create Operations
- [ ] Read / Show Operations
- [ ] Update Operations
- [ ] Delete Operations
- [ ] Confirmation Modals
- [ ] Optimistic UI Updates
- [ ] Pagination
- [ ] Sorting
- [ ] Filtering
- [ ] Searching
- [ ] Bulk Actions
- [ ] Soft Deletes Handling on Frontend
- [ ] Relationship Data Display
- [ ] Nested Resource CRUD
- [ ] Reusable CRUD Components/Patterns

---

# Phase 9 - Tailwind CSS

- [ ] Utility-First Concept
- [ ] Installation via `@tailwindcss/vite` Plugin (v4 — no PostCSS setup needed)
- [ ] CSS-First Configuration (`@import "tailwindcss"`, `@theme` block) — *v4's zero-config approach; replaces the old config file for most projects*
- [ ] *(Legacy Awareness)* `tailwind.config.js` — v3's JS-based config approach, still seen in older codebases
- [ ] Responsive Design Utilities
- [ ] Flexbox Utilities
- [ ] Grid Utilities
- [ ] Spacing & Sizing
- [ ] Typography Utilities
- [ ] Colors & Themes
- [ ] Dark Mode Configuration
- [ ] Reusable Component Classes
- [ ] @apply Directive
- [ ] Plugins (Forms, Typography, Aspect Ratio)
- [ ] Animations & Transitions
- [ ] State Variants (hover, focus, active, disabled)
- [ ] Design Tokens
- [ ] Component Libraries Built on Tailwind

---

# Phase 10 - Inertia.js (Complete Learning Path)

- [ ] What is Inertia.js
- [ ] Why Inertia.js
- [ ] SPA vs Traditional MPA vs Inertia
- [ ] Server-Side Rendering (SSR) Concepts
- [ ] Laravel Backend Setup for Inertia
- [ ] Vue Frontend Setup for Inertia
- [ ] Root Template Setup
- [ ] Rendering Pages from Controllers
- [ ] Shared Data (HandleInertiaRequests Middleware)
- [ ] Layouts
- [ ] Persistent Layouts
- [ ] Link Component
- [ ] usePage Composable
- [ ] useForm Helper
- [ ] Form Submission Handling
- [ ] Validation Error Handling
- [ ] Redirects
- [ ] Flash Messages
- [ ] Partial Reloads
- [ ] Deferred Props
- [ ] Lazy Loading Data
- [ ] Scroll Management
- [ ] Remember State (Local State Persistence)
- [ ] Pagination with Inertia
- [ ] Search Implementation
- [ ] Filtering Implementation
- [ ] Full CRUD with Inertia
- [ ] File Uploads with Inertia
- [ ] Authentication Flow
- [ ] Authorization (Policies/Gates on Frontend)
- [ ] Middleware Interaction
- [ ] Route Model Binding with Inertia
- [ ] Dashboard Development Patterns
- [ ] Performance Considerations
- [ ] Testing Inertia Pages
- [ ] Deployment Considerations
- [ ] Best Practices
- [ ] Common Mistakes & Pitfalls
- [ ] Inertia.js Interview Questions

---

# Phase 11 - Laravel + Vue Integration

- [ ] Laravel API Design for Frontend Consumption
- [ ] API Resources & Resource Collections
- [ ] Sanctum Authentication
- [ ] JWT Authentication
- [ ] CSRF Protection
- [ ] Session vs Token Authentication
- [ ] Authorization (Gates & Policies)
- [ ] Middleware for Frontend Routes
- [ ] File Upload Handling (Backend)
- [ ] Broadcasting Concepts
- [ ] Laravel Echo Setup
- [ ] Pusher Integration
- [ ] Laravel Reverb Basics
- [ ] WebSockets Fundamentals
- [ ] Queues & Frontend Notification Flow
- [ ] Real-Time Notifications
- [ ] Real-Time Chat Features
- [ ] Presence Channels
- [ ] Private Channels

---

# Phase 12 - Enterprise Vue Architecture

- [ ] Feature-Based Folder Structure
- [ ] Domain-Based Folder Structure
- [ ] Components Organization
- [ ] Layouts Organization
- [ ] Services Layer
- [ ] Store Organization
- [ ] Composables Organization
- [ ] Helpers & Utilities
- [ ] Constants Management
- [ ] Centralized Error Handling
- [ ] Logging Strategy
- [ ] Reusable Design Patterns
- [ ] Naming Conventions
- [ ] Scalable Component Design
- [ ] Storybook — isolated component development, visual documentation, design-system consistency across teams
- [ ] Generating Typed API Clients from OpenAPI Specs — bridges your Laravel/Scramble-generated OpenAPI docs directly into typed TS API calls, no manual response typing
- [ ] State Machines (XState) — Awareness — pattern for complex multi-step flows (task status transitions, checkout flows) beyond what a plain store handles well
- [ ] Micro-Frontend Concepts (Awareness)
- [ ] Monorepo Concepts (Awareness)

---

# Phase 13 - Performance Optimization

- [ ] Lazy Loading Components
- [ ] Route-Level Code Splitting
- [ ] Async Component Loading
- [ ] Virtualized Lists
- [ ] Memoization Techniques
- [ ] Avoiding Unnecessary Re-Renders
- [ ] Efficient Watchers
- [ ] Debouncing & Throttling
- [ ] Image Optimization
- [ ] Bundle Size Analysis
- [ ] Tree Shaking
- [ ] Caching Strategies
- [ ] Prefetching & Preloading
- [ ] Web Vitals (LCP, FID, CLS)
- [ ] Lighthouse Auditing
- [ ] Frontend Observability — Sentry (or equivalent) for error tracking, shipping Web Vitals to real analytics in production, not just auditing locally
- [ ] Reducing Reactivity Overhead
- [ ] Production Build Optimization
- [ ] *(Emerging — Awareness Only)* Vapor Mode — Vue's compiler mode that removes the virtual DOM for opted-in components; feature-complete but still labeled unstable as of its latest beta, with Suspense excluded and known friction with Inertia.js page components. Know what it is; don't build production features on it yet.

---

# Phase 14 - Security

- [ ] XSS Prevention
- [ ] CSRF Protection
- [ ] SQL Injection Awareness (Backend)
- [ ] Secure Authentication Practices
- [ ] Secure Token Storage
- [ ] Content Security Policy (CSP)
- [ ] Input Sanitization
- [ ] Output Escaping
- [ ] Secure File Uploads
- [ ] Rate Limiting
- [ ] CORS Configuration
- [ ] Environment Variable Security
- [ ] Dependency Vulnerability Scanning
- [ ] Role-Based Access Control (RBAC)
- [ ] Secure API Design Practices

---

# Phase 15 - Testing

- [ ] Testing Philosophy (Unit vs Integration vs E2E)
- [ ] Vitest Setup
- [ ] Vue Test Utils
- [ ] Unit Testing Components
- [ ] Testing Props & Emits
- [ ] Testing Computed Properties
- [ ] Testing Composables
- [ ] Mocking API Calls
- [ ] Mocking Pinia Stores
- [ ] Integration Testing
- [ ] Snapshot Testing
- [ ] Testing Forms & Validation
- [ ] Testing Router Navigation
- [ ] End-to-End Testing Concepts (Cypress/Playwright)
- [ ] Test Coverage
- [ ] CI Integration for Tests

---

# Phase 16 - Build Tools & Deployment

- [ ] Vite Configuration
- [ ] Environment Variables (.env)
- [ ] Path Aliases
- [ ] Build Optimization
- [ ] Code Splitting Configuration
- [ ] Asset Handling
- [ ] Laravel Mix vs Vite
- [ ] Production Build Process
- [ ] Docker Basics for Laravel + Vue
- [ ] Multi-Stage Docker Builds
- [ ] Nginx Configuration
- [ ] Environment-Specific Builds
- [ ] CI/CD Pipeline Concepts
- [ ] Automated Testing in CI/CD
- [ ] Automated Deployment
- [ ] Zero-Downtime Deployment Concepts

---

# Phase 17 - TypeScript with Vue

- [ ] TypeScript Basics for Vue
- [ ] Typing Props
- [ ] Typing Emits
- [ ] Typing Refs & Reactive State
- [ ] Typing Computed Properties
- [ ] Typing Composables
- [ ] Typing Pinia Stores
- [ ] Generics in Vue Components
- [ ] Type Inference in `<script setup>`
- [ ] Interfaces vs Types
- [ ] Typing API Responses
- [ ] Utility Types
- [ ] Strict Mode Configuration
- [ ] Type-Safe Router
- [ ] Type-Safe Forms

---

# Phase 18 - Nuxt.js Fundamentals

- [ ] What is Nuxt.js
- [ ] When to Use Nuxt vs Vue + Inertia
- [ ] Nuxt Project Structure
- [ ] File-Based Routing
- [ ] Pages & Layouts
- [ ] Server-Side Rendering (SSR)
- [ ] Static Site Generation (SSG)
- [ ] Nuxt Modules
- [ ] Nuxt Data Fetching (useFetch, useAsyncData)
- [ ] Nuxt Middleware
- [ ] Nuxt SEO Basics
- [ ] Nuxt Deployment Basics

---

# Phase 19 - Modern Vue Ecosystem

- [ ] VueUse Utility Library
- [ ] Vue DevTools Usage
- [ ] ESLint Configuration
- [ ] Prettier Configuration
- [ ] Husky Git Hooks
- [ ] Lint-Staged
- [ ] TanStack Query (Vue Query)
- [ ] i18n / Internationalization
- [ ] Accessibility (a11y) Best Practices
- [ ] Progressive Web Apps (PWA)
- [ ] SEO Fundamentals for Vue Apps
- [ ] Chart Libraries Integration
- [ ] Rich Text Editors Integration
- [ ] Drag & Drop Functionality
- [ ] Virtual Scrolling Techniques

---

# Phase 20 - Admin Dashboard Development

- [ ] Authentication Flow for Dashboards
- [ ] Dashboard Layout Structure
- [ ] Sidebar Navigation
- [ ] Navbar & Topbar
- [ ] Data Tables
- [ ] Server-Side Pagination in Tables
- [ ] Charts & Analytics Widgets
- [ ] Filters & Advanced Search
- [ ] CRUD Screens
- [ ] Modals & Dialogs
- [ ] Toast / Notification Systems
- [ ] Permission-Based UI Rendering
- [ ] Role Management Screens
- [ ] Theme Switching
- [ ] Dark Mode Implementation
- [ ] Fully Responsive Layouts
- [ ] Multi-Tenant Dashboard Considerations

---

# Phase 21 - Interview Preparation

## Junior Vue Interview Topics
- [ ] Reactivity Basics
- [ ] Directives
- [ ] Component Basics
- [ ] Props & Events
- [ ] Lifecycle Hooks

## Mid-Level Vue Interview Topics
- [ ] Composition API vs Options API
- [ ] Composables
- [ ] State Management Concepts
- [ ] Router Guards
- [ ] Form Handling Patterns

## Senior Vue Interview Topics
- [ ] Reactivity System Internals
- [ ] Performance Optimization Strategies
- [ ] Architecture Decisions
- [ ] Scalability Patterns
- [ ] Render Function / Virtual DOM Concepts

## Laravel + Vue Interview Topics
- [ ] API Design Best Practices
- [ ] Authentication Strategies Comparison
- [ ] Real-Time Feature Implementation
- [ ] Error Handling Across Stack

## Inertia.js Interview Topics
- [ ] Inertia Request Lifecycle
- [ ] Partial Reloads Explanation
- [ ] SSR with Inertia
- [ ] Common Inertia Pitfalls

## Pinia Interview Topics
- [ ] Store Design Patterns
- [ ] Pinia vs Vuex
- [ ] Store Composition Strategies

## Vue Router Interview Topics
- [ ] Guard Execution Order
- [ ] Dynamic Route Matching
- [ ] Lazy Loading Strategy

## Performance Interview Topics
- [ ] Identifying Bottlenecks
- [ ] Optimization Techniques
- [ ] Bundle Size Reduction Strategies

## Architecture Interview Topics
- [ ] Folder Structure Justification
- [ ] Scalable Component Design
- [ ] Separation of Concerns
- [ ] Store vs State Machine — when a Pinia store is enough vs when a formal state machine (XState) earns its complexity
- [ ] Typed Contracts Between Frontend & Backend — OpenAPI-generated clients vs hand-maintained types, and the tradeoffs

## Scenario-Based Interview Topics
- [ ] Debugging Reactivity Issues
- [ ] Handling Large Data Sets in UI
- [ ] Designing a Multi-Tenant Dashboard
- [ ] Migrating a Legacy App to Vue + Inertia
- [ ] Optimizing a Slow Admin Panel
