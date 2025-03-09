# Pilgrim Passport Software Requirements Doc

# Software Requirements Specification

## System Design
- Progressive Web App (PWA)
- Server-Side Rendering (SSR) with Next.js
- Edge Functions for QR code processing
- Real-time updates for achievements
- Offline capability for basic functions
- CDN for static assets and images

## Architecture Pattern
- Next.js App Router architecture
- Server Components for improved performance
- Client Components for interactive features
- Middleware for authentication/authorization
- API Routes for backend functionality
- Edge Runtime for global distribution

## State Management
- Server State: React Query/TanStack Query
- Client State: React Context API
- Form State: React Hook Form
- Persistent State: Local Storage
- Real-time State: Supabase Realtime

## Data Flow
1. Authentication Flow:
   - Email/Password signup
   - Email verification
   - Session management
   - Password reset

2. Visit Recording Flow:
   - QR code scan
   - Geolocation verification
   - Visit timestamp
   - Achievement check
   - Notification dispatch

3. Data Sync Flow:
   - Real-time updates
   - Offline data storage
   - Background sync
   - Conflict resolution

## Technical Stack
- Frontend:
  * Next.js 14+
  * TypeScript
  * Tailwind CSS
  * PWA manifest
  * Service Workers

- Backend:
  * Supabase
  * Edge Functions
  * Storage Buckets
  * Real-time subscriptions

- DevOps:
  * Vercel deployment
  * GitHub Actions
  * Environment management
  * Monitoring/Analytics

## Authentication Process
- Supabase Auth implementation
- JWT token management
- Role-based access control
- Session handling
- Security middleware
- Rate limiting

## Route Design
```typescript
/app
  ├── (auth)
  │   ├── login
  │   ├── register
  │   └── reset-password
  ├── (dashboard)
  │   ├── profile
  │   ├── parishes
  │   ├── achievements
  │   └── visits
  ├── (admin)
  │   ├── parishes
  │   ├── reports
  │   └── users
  └── api
      ├── auth
      ├── parishes
      ├── visits
      └── achievements
```

## API Design
- RESTful endpoints:
  ```typescript
  /api/auth/*
  /api/parishes/*
  /api/visits/*
  /api/achievements/*
  /api/reports/*
  ```
- WebSocket connections:
  * Real-time visit updates
  * Achievement notifications
  * Admin dashboard updates

## Database Design ERD
```markdown
Users
  - id (UUID)
  - email
  - profile_data (JSON)
  - created_at
  - last_login

Parishes
  - id (UUID)
  - name
  - location
  - history
  - mass_times (JSON)
  - qr_code
  - media_urls

Visits
  - id (UUID)
  - user_id (FK)
  - parish_id (FK)
  - timestamp
  - verification_data

Achievements
  - id (UUID)
  - name
  - description
  - criteria (JSON)
  - icon_url

UserAchievements
  - user_id (FK)
  - achievement_id (FK)
  - earned_at
  - metadata (JSON)

Reports
  - id (UUID)
  - type
  - data (JSON)
  - generated_at
```
```

