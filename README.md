# Collab-write – Real-time Collaborative Editor

A real-time collaborative text editor that allows multiple users to edit documents simultaneously with live updates, comments, and role-based access control.

**Live Demo:** https://collab-write-topaz.vercel.app/  
**GitHub Repo:** https://github.com/durgax04/Collab-write

---

## Features

- Real-time multi-user editing (sub-second latency)
- Live text selection & inline comments
- Presence awareness (see active collaborators)
- Authentication & session management (Clerk)
- Role-based access control (Admin/User permissions)
- Document sharing & collaboration
- Clean and responsive UI

---

## Tech Stack

- **Frontend:** Next.js (App Router), TypeScript, Tailwind CSS  
- **Realtime Engine:** Liveblocks  
- **Authentication:** Clerk  
- **State & UI:** React, Custom Hooks  

---

## Architecture Overview

- Liveblocks handles real-time sync using WebSocket-based infrastructure  
- Clerk manages authentication and secure sessions  
- Role-based access ensures only authorized users can edit/view documents  
- Optimized rendering for smooth collaborative experience  

---

## Getting Started
### 1. Clone the repository

```bash
git clone https://github.com/durgax04/Collab-write.git
cd Collab-write
```
### 2. Install dependencies
```bash
pnpm install
```

### 3. Create a .env file
```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/signin
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/signup

LIVEBLOCK_SECRET=
```

### 4. Run the development server
```bash
pnpm dev
```

