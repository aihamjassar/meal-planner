# Meal Planner

> An in-progress Next.js meal-planning and food-management application with authentication support, Prisma-backed data access, dashboard routing, and category-management workflows.

## Overview

This repository contains the source and supporting files for **Meal Planner**. The documentation below was prepared from the current repository structure and implementation files so that setup expectations, project boundaries, and implemented capabilities are explicit.

## Technology

| Area | Implementation |
| --- | --- |
| Framework | Next.js 15 and React 19 |
| Data | Prisma ORM with PostgreSQL |
| Authentication | NextAuth dependency and application providers |
| State and forms | Zustand, React Hook Form, and Zod |

## Key capabilities

| Area | Current implementation |
| --- | --- |
| Dashboard foundation | Organizes application routes around an authenticated dashboard. |
| Food-category management | Includes category cards and a category-form dialog. |
| Typed data layer | Uses Prisma, service helpers, and schema types. |

## Getting started

Use the following workflow to work with the project locally.

```bash
git clone https://github.com/aihamjassar/meal-planner.git
cd meal-planner
npm install
# Set database and auth environment values
npm run db:migrate
npm run dev
```

## Project structure

| Path | Purpose |
| --- | --- |
| prisma/ | Prisma schema and migration files |
| src/app/(dashboard)/ | Dashboard and administration routes |
| src/app/(dashboard)/admin/foods-management/categories/ | Category-management screen |
| src/services/ | Query and mutation helpers |
| src/store/ | Global and category state stores |

## Configuration notes

Set the database and authentication configuration before running migrations. The currently visible implementation emphasizes administrative category management; document additional meal-planning flows as they are completed.

## License

No license file is currently included. Confirm the intended licensing terms with the repository owner before reuse or distribution.

## Maintainer

Maintained by [Aiham Jassar](https://github.com/aihamjassar). Contributions, issue reports, and improvement suggestions are welcome through the repository.
