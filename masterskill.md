---
name: master-web-sql-builder
description: Build compact, professional HTML/CSS/JS/SQL websites and business apps. Use for static/core HTML CSS JS SQL sites, ERP, CRM, analytics dashboards, CRUD systems, root/public structure, responsive UI, header/sidebar/footer placement, auth/user/role flows, accessibility, performance, SQL schema/query design, PlanetScale/MySQL/Postgres/Vitess/Neki guidance, Laravel AI SDK features, terse reviews, and concise delivery.
---

# Master Web SQL Builder

Use simplest correct solution. Remove filler, hedging, and duplicate words. Preserve technical meaning, code, commands, paths, URLs, names, dates, versions, and error text exactly.

## Compression Principle

Compress long skills into rules that preserve action and accuracy. Example: caveman skill becomes "Remove filler, hedging, and unnecessary words while preserving full technical meaning and code accuracy." Keep trigger, rule, numbers, exceptions; delete history, repetition, and decorative examples.

## Default Workflow

1. Read request, existing files, and data model before building.
2. Choose plain HTML/CSS/JS/SQL unless project already uses a framework.
3. Build mobile-first, then tablet, then desktop.
4. Keep root minimal; put assets and mutable files in `public/`.
5. Use semantic HTML, accessible controls, responsive CSS, efficient JS, measured SQL.
6. Verify layout, keyboard use, contrast, forms, console errors, query shape, and file paths.
7. Deliver concise summary plus exact files changed.

## Website/App Types

- Landing/marketing: hero, proof, features, pricing/offer, FAQ, contact, footer.
- Content/blog/docs: readable article layout, search, categories, table of contents, related content.
- E-commerce: catalog, product detail, cart, checkout, orders, account, email/status states.
- SaaS app: dashboard, records, settings, billing, users, roles, audit log.
- CRM: leads, contacts, companies, deals, pipeline, tasks, notes, communication history.
- ERP: inventory, purchasing, sales, finance, HR, projects, approvals, reports, audit.
- Analytics: KPIs, charts, filters, date ranges, drilldown, export, saved views.
- Admin panel: users, roles, config, logs, imports, approvals, destructive controls.

## File Layout

Root holds core files only:

- `index.html`
- `style.css`
- `script.js`
- `schema.sql` or `database.sql` when SQL is needed
- optional config only if required

`public/` holds everything else:

- `public/assets/`
- `public/images/`
- `public/fonts/`
- `public/vendor/`
- `public/data/`
- `public/uploads/`

Assume root may become read-only after delivery. Keep runtime writes, generated media, user uploads, caches, and large assets out of root.

## HTML Rules

- Use landmarks: `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`.
- Use one `h1`; keep heading order sequential.
- Add `<meta name="viewport" content="width=device-width, initial-scale=1">`; never disable zoom.
- Use real buttons for actions and links for navigation.
- Give every input a visible `label`; never use placeholder as only label.
- Add `alt` to meaningful images; empty `alt=""` for decorative images.
- Add `aria-label` to icon-only buttons; expose expanded/selected/disabled state.
- Add skip link for content-heavy pages.
- Keep DOM order equal to reading/focus order.

## CSS System

- Use tokens: colors, spacing, radius, shadows, z-index, typography.
- Spacing scale: `4, 8, 12, 16, 24, 32, 48, 64, 96, 128`.
- Radius: buttons/cards usually `4-8px`; avoid oversized rounded cards unless brand requires.
- Shadows: one small scale; no random shadow values.
- Type: body `16px`, line-height `1.5-1.75`, headings `600-700`, labels `500`.
- Use breakpoint tokens, not viewport-width font scaling.
- Keep letter spacing `0` unless all-caps label needs slight spacing.
- Use semantic color names: `surface`, `text`, `muted`, `primary`, `danger`, `success`, `border`.
- Contrast: normal text `4.5:1`, large text/UI borders `3:1`.
- Do not rely on color alone; pair state color with icon/text.
- Use one icon family; prefer SVG/Lucide/Heroicons; do not use emoji as UI icons.
- Animate only `transform` and `opacity`; duration `150-300ms`; support `prefers-reduced-motion`.

## Responsive Layout

Breakpoints:

- phone: `360-480px`
- tablet: `768px`
- laptop: `1024px`
- desktop: `1280-1440px`

Containers and gutters:

- mobile content gutter: `16px`
- tablet gutter: `24-32px`
- desktop gutter: `40-64px`
- normal max-width: `1120-1200px`
- wide/data max-width: `1280-1440px`
- text measure: mobile `35-60` chars, desktop `60-75` chars

Section rhythm:

- mobile section padding: `48-64px`
- tablet: `72-96px`
- desktop: `96-128px`
- component gap: `8-16px`
- card/grid gap: `16px` mobile, `24px` tablet, `32px` desktop

Grid:

- mobile: 1 column
- tablet: 2 columns
- desktop: 3-4 columns
- dashboards: sidebar at `1024px+`; top/bottom nav on small screens
- forms: single column on mobile, two columns only when fields naturally pair

No horizontal scroll. Reserve space for fixed headers/footers. Prefer `min-height: 100dvh` over `100vh` on mobile.

## 1% Layout Placement

- Public/marketing site: top header, main sections, footer. No sidebar.
- SaaS/app/dashboard: top utility header plus left sidebar on desktop. No footer unless legal/support links are required.
- Admin/CRM/ERP: persistent left sidebar, top bar for search/actions/user, dense main table/detail area.
- E-commerce: header with logo, search, account, cart; footer required.
- Blog/docs: header, optional left table-of-contents/sidebar on desktop, centered readable content, footer.
- Mobile app-like web: top bar or bottom nav with 3-5 primary items; sidebars become drawer/sheet.

## Header

- Position: top of page/app, full width, `56-72px` high desktop, `56-64px` mobile.
- Public header content: logo/name, primary nav, primary CTA, login, optional search.
- App header content: page title/breadcrumb, global search, create/action button, notifications, user menu.
- Mobile header: logo/title, one primary action, menu/user icon. Move low-priority nav into drawer.
- Sticky header only when navigation/action must stay available. Reserve top padding so content is not hidden.
- Avoid crowded headers. If more than 5 nav items, group under menu or sidebar.

## Sidebar

- Use sidebar for logged-in apps, admin panels, dashboards, docs, settings, and multi-section tools.
- Do not use sidebar for simple landing pages, checkout, auth pages, or one-page marketing sites.
- Desktop position: left side, `240-280px` wide, sticky/fixed, usually below top header.
- Full-height app shell: sidebar may start at top with logo; header begins to its right.
- Mobile: sidebar becomes drawer/sheet; keep current section visible in header or bottom nav.
- Sidebar content: logo/workspace, primary modules, secondary settings, collapse control, role/tenant switcher if needed.
- Right sidebar: use only for contextual details, help, filters, inspector, or activity. Never primary navigation.

## Footer

- Use footer for public, marketing, content, e-commerce, legal, and trust-heavy pages.
- Omit or minimize footer in dashboards/admin apps; logged-in tools should prioritize workspace, not repeated legal links.
- Usual footer content: copyright, terms, privacy, contact/support, key nav, social links, address, status, newsletter if real.
- Footer placement: after main content, full width, visually quieter than main CTA, enough top padding to separate.
- Mobile footer: stacked groups, large tap targets, no tiny inline link soup.

## Page Sections

- Hero: product/offer visible first viewport; H1, short proof, primary CTA, secondary action only if useful; next section peeks.
- Feature grid: 3-6 features, icon + title + 1-2 lines; no paragraph walls.
- Dashboard/data: dense, scannable, restrained; tables, filters, tabs, status chips, pagination.
- Pricing: 2-4 plans; highlight one recommended plan; compare concrete limits.
- Testimonials/logos: use real names/logos only when available; otherwise omit.
- FAQ: accordion only for secondary questions.
- Contact/form: labels, helper text, inline errors, success state, retry path.

## Business App Shell

- App default: sidebar modules, top bar search/actions/user, main content, optional right inspector.
- Main content order: title/breadcrumb, primary action, KPI/summary row, filters, table/list/chart, pagination.
- Use tabs for sibling views of one record; use sidebar for modules; use breadcrumbs for depth.
- Keep primary action top-right (`New`, `Save`, `Approve`, `Export`) and destructive actions in overflow/detail area.
- Show empty, loading, error, no-permission, no-results, archived, and offline states.
- Every list needs search, filters, sort, pagination, selected/bulk state, export if business data.
- Every record needs view, create, edit, delete/archive, status, owner, timestamps, history/audit.
- Prefer archive/soft-delete for business records; hard delete only for safe temporary data.
- Use status chips with text: draft, active, pending, approved, rejected, archived, paid, overdue.

## Data Tables

- Desktop: table for dense business data; sticky header for long tables; first column identifies record; actions right.
- Mobile: convert to cards or priority columns; keep search/filter/action available.
- Columns: stable order, left-align text, right-align numbers/money, use tabular numbers.
- Include: row checkbox only when bulk actions exist; visible sort state; row count; page size.
- Filters: date range, status, owner/team, category/type, amount range, free search, saved filters.
- Row actions: view/edit primary, secondary in menu; destructive separated and confirmed.
- Bulk actions: select all current page, clear selection, show selected count, confirm destructive bulk changes.
- Exports: CSV for tables, PDF only for human-readable documents, chart image only when useful.
- Avoid: table inside card inside card, hidden horizontal scroll without indicator, color-only statuses.

## Forms And CRUD

- CRUD flow: list -> create/edit -> validate -> save -> success -> detail/list.
- Form layout: one column mobile; grouped sections desktop; labels always visible; required fields marked.
- Put primary save action in header/footer sticky area for long forms; secondary cancel/back nearby.
- Validate on blur and submit. Error text states cause and fix. Focus first invalid field.
- Autosave drafts for long/high-value forms; warn before leaving unsaved changes.
- Inputs: use correct type (`email`, `tel`, `number`, `date`, `search`), autocomplete, masks only when helpful.
- Selects: use searchable select for 20+ options; async lookup for large datasets.
- File upload: type/size limit, progress, preview, remove, retry, server validation.
- Record detail: summary header, key fields, activity, related records, attachments, comments/notes.

## ERP Patterns

- Core modules: inventory, products/SKUs, vendors, purchase orders, sales orders, invoices, payments, employees, approvals, reports.
- Inventory: product, SKU, warehouse, stock movement, quantity on hand, reserved, reorder level, cost.
- Purchasing: vendor -> purchase order -> receipt -> bill -> payment.
- Sales: customer -> quote/order -> shipment/service -> invoice -> payment.
- Finance: invoice, payment, account, tax, discount, adjustment, ledger/audit trail.
- Approval flow: draft -> submitted -> approved/rejected -> posted/locked. Record who, when, comment.
- Do not edit posted financial/stock records silently; create adjustment/reversal records.
- ERP UI prioritizes accuracy, auditability, filters, exports, and role-safe actions over decorative design.

## CRM Patterns

- Core modules: leads, contacts, companies/accounts, deals/opportunities, pipeline, tasks, notes, calls/emails, campaigns.
- Pipeline: stages, probability, expected value, close date, owner, next action.
- Lead flow: new -> contacted -> qualified -> converted/lost. Conversion creates contact/company/deal.
- Contact/company detail: timeline first, then open deals, tasks, notes, emails/calls, files.
- CRM list filters: owner, stage, source, status, last activity, next due, created date, value.
- Require next action on active deals/leads; surface stale records and overdue tasks.
- Avoid duplicate people/companies: normalize email/domain/phone; show merge path.

## Analytics Patterns

- Dashboard top row: 3-6 KPIs with value, delta, period, comparison baseline.
- Controls: date range, segment, status, owner/team, region/product, refresh/export.
- Charts: trend -> line, comparison -> bar, composition -> stacked/donut only <=5 categories, funnel -> funnel/bar, geography -> map plus table.
- Every chart needs title, unit, date range, empty/loading/error state, accessible summary, table/export fallback.
- Drilldown: KPI -> chart -> filtered table -> record detail.
- Use consistent number formatting: currency, percent, compact counts, dates by locale.
- Avoid vanity charts, 3D charts, pie charts with many categories, color-only legends, unlabeled axes.
- Analytics SQL should use date spine/calendar for missing periods and pre-aggregations for heavy dashboards.

## Interaction

- Touch/click targets: minimum `44x44px`; keep `8px+` gap.
- Show hover, focus, pressed, loading, disabled, success, and error states.
- Feedback within `100ms`; skeleton/progress if load exceeds `300ms`.
- Disable submit during async work; preserve input on failure.
- Confirm destructive actions; offer undo when practical.
- Modals need title, close button, focus trap, Escape close, and focus return.
- Navigation must preserve scroll/filter/form state when returning.

## Users, Login, Roles

- Public state: header shows `Login` plus one main CTA (`Sign up`, `Book`, `Get started`, `Contact`).
- Guest state: can browse public data only; protected actions redirect to login with return URL.
- Auth pages: simple centered form, logo, email/password, password toggle, forgot password, submit state, signup/login switch. No heavy nav/sidebar.
- Logged-in header: avatar/name, profile, settings, billing/workspace, help, logout.
- User table: `id`, `name`, `email`, `password_hash`, `email_verified_at`, `last_login_at`, `status`, timestamps.
- Role model: `roles`, `permissions`, `role_user`, optional `permission_role`. Keep permissions server-side.
- Common roles: owner, admin, manager, staff, user, guest.
- Owner: billing, delete workspace, transfer ownership. Admin: users, settings, roles. Manager: team/workflow. Staff: assigned operations. User: own data. Guest: limited read.
- UI may hide forbidden actions; backend must enforce every permission.
- Multi-tenant apps: every scoped table has `organization_id` or `account_id`; every query filters by tenant and permission.
- Access failure: unauthenticated goes to login; authenticated without permission gets 403/request-access/upgrade path.
- Audit role, permission, billing, export, delete, and password/security changes.

## Notifications And Activity

- Use notifications for assigned, approved/rejected, failed import/export, overdue, comment mention, payment/order status.
- Notification item: actor, action, object, time, unread state, link to record.
- Activity feed: immutable event log for business actions; comments are separate editable/deletable records.
- Email/SMS/push preferences per user; critical security/transaction notices cannot be fully disabled.

## JavaScript

- Keep JS modular and small; no framework unless needed.
- Use event delegation for repeated items.
- Debounce search/resize/scroll.
- Use `defer` for scripts; avoid blocking initial render.
- Lazy-load non-critical modules/media.
- Validate on blur and submit; never trust client validation alone.
- Use `fetch` with timeout, error state, loading state, and retry where useful.
- Sanitize untrusted HTML; prefer text insertion over `innerHTML`.
- Store only safe client data; never expose secrets in frontend.
- For business apps, keep client state explicit: current user, tenant, route/view, filters, sort, page, selected rows, dirty form, loading/error.
- Persist harmless preferences: sidebar collapsed, theme, table columns, saved filters. Do not persist secrets.

## Performance

- Use AVIF/WebP when possible; provide width/height or `aspect-ratio`.
- Lazy-load below-fold images; preload only critical fonts/assets.
- Use `font-display: swap` or `optional`.
- Avoid layout shifts: reserve space for media, cards, tables, ads, and async content.
- Keep per-frame work under `16ms`; avoid layout read/write loops.
- Virtualize lists over ~50 visible-heavy items.
- Remove unused vendor files; load third-party scripts `async`/`defer`.
- Check console, network 404s, mobile viewport, and slow network behavior.

## Accessibility

- Keyboard can complete all tasks.
- Focus ring visible; never remove outline without replacement.
- Focus moves to main content after page changes and to first invalid field after submit.
- Use `aria-live="polite"` for async success/error messages.
- Charts need text summary and table alternative.
- Media needs captions/transcripts when speech matters.
- Do not flash more than 3 times per second.
- Test at 200% text zoom and small phone width.

## SQL Design

- Start from entities, relationships, cardinality, read/write patterns, and expected scale.
- Normalize to 3NF first; denormalize only for proven hot reads.
- Use `snake_case`; keep names clear and consistent.
- Prefer `BIGINT` IDs: MySQL `BIGINT UNSIGNED AUTO_INCREMENT`; Postgres `BIGINT GENERATED ALWAYS AS IDENTITY`.
- Avoid random UUID primary keys. If public IDs needed, keep UUID/ULID as secondary unique column.
- Add `NOT NULL` wherever valid.
- Add `created_at` and `updated_at`; use MySQL `DATETIME`, Postgres `TIMESTAMPTZ`.
- Money: `DECIMAL(19,4)` or integer cents; never float.
- MySQL: use `utf8mb4` / `utf8mb4_0900_ai_ci`.
- Postgres: prefer `TEXT`, `JSONB` when needed, `CHECK` over hard-to-change enum types.
- JSON only for dynamic attributes; index extracted fields/generate columns when queried.
- Foreign keys: define delete behavior; index FK columns, especially in Postgres.
- Business tables usually include: `id`, tenant key, human number/code, status, owner/user, timestamps, created_by, updated_by.
- Use separate tables for notes, attachments, activities, audit logs, tags, comments, status history.
- Use immutable ledger/movement tables for inventory, payments, approvals, and audit-critical events.

## SQL Modules

- Auth: `users`, `roles`, `permissions`, `role_user`, `permission_role`, `sessions`, `password_resets`.
- Tenant: `organizations/accounts`, `organization_user`, `plans`, `subscriptions`, `billing_events`.
- CRM: `leads`, `contacts`, `companies`, `deals`, `deal_stages`, `tasks`, `notes`, `activities`.
- ERP inventory: `products`, `skus`, `warehouses`, `stock_movements`, `vendors`, `purchase_orders`, `purchase_order_items`.
- ERP sales/finance: `customers`, `sales_orders`, `sales_order_items`, `invoices`, `invoice_items`, `payments`, `tax_rates`.
- Analytics: source tables plus `daily_metrics`/materialized summary tables for heavy dashboards.
- System: `audit_logs`, `notifications`, `files`, `imports`, `exports`, `settings`.

## SQL Indexes

- Index columns used in `WHERE`, `JOIN`, `ORDER BY`, and frequent filters.
- Composite order: equality columns first, then range, then sort.
- Respect leftmost-prefix rule.
- Range predicates stop later columns from filtering well.
- Prefer one useful composite index over many weak single-column indexes.
- Covering indexes help only when selected columns are narrow and stable.
- Do not over-index write-heavy tables.
- Audit unused/duplicate indexes before dropping; get approval before destructive changes.
- Business app default composite indexes: `(tenant_id, status)`, `(tenant_id, created_at)`, `(tenant_id, owner_id)`, `(tenant_id, deleted_at)`, plus module-specific lookup keys.
- Analytics indexes often start with date/time and tenant/segment keys; test with actual dashboard queries.

## SQL Queries

- Select needed columns; avoid `SELECT *`.
- Use cursor pagination; avoid deep `OFFSET`.
- Avoid functions/arithmetic/casts on indexed columns in `WHERE`.
- Avoid leading wildcard `LIKE '%term'`; use prefix/full-text/search engine.
- Replace N+1 loops with joins, eager loading, or batched `IN/ANY`.
- Use `UNION ALL` when dedupe is unnecessary.
- Add `LIMIT` to unbounded reads.
- Use `EXPLAIN` / `EXPLAIN ANALYZE`; fix full scans, filesort/temp tables, high rows-read/rows-returned.
- Keep transactions short; do external I/O outside transactions.
- Lock rows in consistent order; retry deadlocks with backoff.
- Ask before dropping, truncating, deleting, detaching partitions, or resetting stats.
- For dashboards, aggregate on server/SQL, not by pulling all rows to JS.
- For money/inventory, wrap multi-row writes in transactions and write audit/movement rows atomically.
- For reports, keep filters sargable and export from the same filtered query users see.

## Imports, Exports, Reports

- Import flow: upload -> validate -> preview errors -> confirm -> process -> result log.
- Store imports with file, user, row count, success/error count, timestamp, mapping.
- Export flow: current filters -> confirm scope -> generate -> download link -> audit event.
- Reports need title, period, filters, generated time, totals, detail table, export.
- Large imports/exports run async with progress and notification.
- Never allow export to bypass role/tenant permissions.

## Scaling Databases

- MySQL/Vitess: design vindex/shard key early; filter by shard key; avoid cross-shard joins and cross-shard locking.
- Vitess: use Online DDL/deploy requests; use sequences or app-generated IDs for sharded tables; do not rely on triggers/procedures through VTGate.
- Sharded Postgres/Neki: design tenant/shard key early; keep related rows colocated; avoid global uniqueness that blocks sharding.
- Partition only large/time-series tables or retention-heavy data; partition key must be in unique/primary keys.
- Use pooling; do not raise max connections reactively.
- Plan rollback and post-deploy verification for production schema changes.

## Laravel AI SDK

Use only when project references `ai-sdk`, `laravel/ai`, `Laravel\Ai\`, agents, RAG, embeddings, streaming, tools, or provider failover.

- Search package docs before coding; do not guess new APIs.
- Text/chat: Agent class + `Promptable`.
- Memory: `Conversational` or `RemembersConversations`.
- JSON: `HasStructuredOutput`.
- Tools: `HasTools`; scaffold with `php artisan make:tool`.
- Images/audio/transcription/embeddings/reranking/files/stores: use SDK facades and test fakes.
- Provider features differ; guard unsupported capabilities.
- Use failover for production reliability.
- Tests must fake AI calls; never hit live providers in normal tests.

## Review And Commit Style

- Reviews: lead with bugs/risks. Format: `file:line: problem. fix.`
- Commits: Conventional Commits. Subject imperative, <=50 chars when possible, <=72 hard cap.
- Add commit body only for why, breaking changes, migrations, security fixes, reverts, or issue refs.
- No AI attribution, emoji, filler, or restating obvious file changes.

## Delivery Checklist

- Files follow root/public layout.
- Mobile/tablet/desktop checked: no overlap, no horizontal scroll, readable text.
- Buttons/forms/navigation accessible by keyboard and touch.
- Contrast, labels, alt text, focus, loading, empty, error, success states present.
- ERP/CRM/analytics screens include filters, status states, permissions, audit/history, export/import where expected.
- Images sized/lazy/optimized; scripts deferred; no console errors.
- SQL schema has correct keys, types, constraints, indexes, and rollback plan.
- Output concise: what changed, where, how verified.
