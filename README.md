# Cmane1
Habit tracker 
# Run Habit Tracker (Expo + React Native)

A minimal mobile habit tracker to log your runs. Built with Expo and plain JavaScript for a simple beginner-friendly workflow.

Features (MVP)
- Add a run: date, distance (km), duration (minutes), notes
- View runs (most recent first)
- Edit and delete runs
- Simple summary: total distance, total duration, current streak
- Export / Import JSON backup
- Local persistence via AsyncStorage (no backend required)

Getting started
1. Install Expo CLI (if needed)
   - npm install -g expo-cli

2. Install dependencies
   - npm install

3. Start the project
   - npm run start
   - Open the project in Expo Go (scan the QR code) or an emulator

Project structure
- App.js — main app container and state
- src/components/RunForm.js — form to add/edit runs
- src/components/RunList.js — list of runs with edit/delete
- src/components/Summary.js — simple stats and streak
- src/utils/storage.js — AsyncStorage helpers, export/import

Data model
A run object:
{
  id: string,
  date: "YYYY-MM-DD",
  distanceKm: number,
  durationMin: number,
  notes: string
}

Next steps / ideas
- Add a date picker component for easier date entry
- Add charts (distance over time) using a chart library
- Turn into a PWA or add cloud sync (Supabase / Firebase)
- Add GPS route integration (advanced)

If you want, I can:
- Add TypeScript types and convert the project
- Add an easy date picker
- Scaffold CI / GitHub repo files
