# Growth & Elevation — College Readiness

Grade 12 English web app for Mr. Isaiah.

## Current setup
- Supabase authentication via Google OAuth
- Supabase database for assignments, submissions, grades, and profiles
- Head admin is determined by the `admins` table / profile role
- Supabase publishable key is used in the browser; no service-role secret is included

## Deployment
This project can be deployed to Vercel or another Node host. The Supabase project is already configured for Google OAuth. Set the deployed site's URL as an allowed redirect URL in Supabase Auth URL Configuration when deploying.

## Important
The Supabase publishable key is intentionally included in the browser code. Never place a Supabase secret/service-role key in `public/index.html` or any client-side code.
