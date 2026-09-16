# DOJO 

A gamified task assistant built for people with ADHD and executive dysfunction. DOJO breaks big tasks into small steps, then uses photo verification to confirm each step actually got done.

## Features

- **Task breakdown** – Turn a vague task into clear, actionable steps using AI decomposition
- **Photo verification** – Snap a live photo to prove a step is complete (no gallery uploads, so no cheating)
- **Gamification** – Earn points, build streaks, and unlock badges as you complete tasks
- **Progress tracking** – See your history, levels, and milestones over time

## Tech Stack

- **Frontend:** HTML, CSS (Bootstrap), JavaScript — responsive for phone and tablet
- **Backend:** Flask (Python), hosted on Render
- **Database:** Supabase (Postgres)
- **AI:** Groq API — one text model for task decomposition, one vision model for photo verification
- **Image handling:** Pillow + imagehash for duplicate photo detection

## Setup

1. Clone the repo
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set environment variables:
   - `GROQ_API_KEY`
   - `SUPABASE_KEY`
4. Run locally:
   ```bash
   flask run
   ```

> Note: keep your `.env` file gitignored — never commit secrets.

## Database Schema

Core tables: `users`, `tasks`, `steps`, `completions`, `gamification`, `logs`

## Build Order (MVP → Full)

1. Task/step engine + Supabase storage (no camera/AI yet)
2. Gamification (points, streaks, badges)
3. Live photo capture + perceptual hash check
4. Groq vision verification
5. Groq text task decomposition

## Status

**Done:**
- Icons, login screen, colour palette
- 16 badge medallion assets (SVG)

**Still to build:**
- Sign Up / Forgot Password screens
- Dashboard, Task List, Task Detail
- New Custom Task, Step Execution, Photo Capture, Verification Result
- Progress/Badges screen, Level-up screen
- Profile/Settings, History/Logs

**Assets still needed:**
- App icon/favicon, splash screen
- Empty-state illustrations, loading spinner
- Error states (camera denied, offline/API failure)
- Locked-badge treatment, notification icon

## Distribution

Target: PWABuilder or Capacitor for an installable Android app via Google Play (~$25 one-off fee). No plans for Apple App Store.
