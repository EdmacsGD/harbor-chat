# Harbor Chat

A Discord-style chat app in one HTML file. Made by Edvards Macs.

- Text channels, DMs, display names, colors and avatars
- Image sharing, emoji reactions, edit and delete your own messages
- Live updates with Supabase Realtime

## How it works

- Frontend: `index.html` (plain HTML, CSS, JavaScript)
- Backend: Supabase (Postgres + anonymous sign-in + Realtime)
- Security: Row Level Security. You can only edit your own messages and profile, and DMs are only readable by the two people in them.

The key in `index.html` is a publishable key. It is safe to be public because the database rules decide what each user can do.
