---
name: Feature Request
about: Suggest a new feature or improvement.
title: "[FEATURE] "
labels: enhancement
assignees: ''
---

## Feature Description  
Implement the *Admin Dashboard* where administrators can manage polls, users, categories, and reported posts.

## Problem It Solves  
Currently, the application only supports the user-facing landing page.  
There is *no admin interface* to:  
- create/edit/delete polls  
- manage users  
- moderate content  
- view overall statistics

This makes the system incomplete.

## Proposed Solution  
Build a secure admin dashboard with:  
- Login authentication (JWT + role-based auth)  
- Poll management CRUD  
- User management CRUD  
- Analytics section (total polls, votes, active users)  
- Approve/Reject reported posts

Frontend: React + Tailwind  
Backend: New /admin routes in Express  
DB: New tables (admin_activity_logs, reports, etc.)

## Alternatives Considered  
- Managing everything through pgAdmin (not user-friendly)  
- Using a prebuilt CMS dashboard (not flexible enough)

## DevOps Impact  
- Requires new CI/CD jobs for admin frontend  
- Requires database migrations in DevOps pipeline  
- Requires new environment variables (JWT secrets, RBAC roles)  
- Admin should have separate staging environment for testing
