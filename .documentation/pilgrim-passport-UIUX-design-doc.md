# Pilgrim Passport UI/UX Design Doc

# Updated User Interface Design Document - Parish Visit Tracking System

## Layout Structure
- Seamless integration within existing Diocese website
- Consistent header/footer with main Diocese website
- Clear section indicating "Pilgrim Passport" area
- Hierarchical navigation showing user's location within the system

## Core Components

### Welcome/About Section
- Hero section explaining Jubilee Year celebration
- Visual onboarding flow
- Quick-start guide
- Benefits overview
- Getting started button

### Onboarding Wizard
- Step-by-step guided setup:
  1. Account creation
  2. Profile setup
  3. Privacy preferences
  4. QR code scanning tutorial
  5. Parish browsing introduction
- Progress indicator
- Skip option for experienced users
- Help tooltips

### Main Dashboard
- Welcome message
- Visit statistics summary
- Recent achievements
- Nearby parishes
- Quick actions:
  * Scan QR Code
  * View Passport
  * Browse Parishes
  * Achievement Gallery

### Parish Passport Collection
- View toggle (Grid/List/Map)
- Search and filter options
- Sort by:
  * Alphabetical
  * Visit date
  * Distance
  * Recently added
- Visit status indicators:
  * Visited (with date)
  * Not yet visited
  * Special events

## Parish Visit Display - Detailed Design

### List/Grid Toggle
- Prominent view toggle in the top-right of parish listing
- Remembers user's last selected view preference

### Grid View
- Parish cards (responsive sizing)
- Components:
  * Parish photo/image
  * Parish name (prominent)
  * Visit status badge (top-right corner)
    - "Not Visited" - subtle gray badge
    - "Visited" - colored badge with date
  * Quick-view information:
    - City/Location
    - Next mass time
    - Distance (if location enabled)
  * Click/tap anywhere on card to expand

### List View
- Single-column layout
- Components per row:
  * Small parish thumbnail
  * Parish name and location
  * Visit status indicator
  * Next mass time
  * Expandable preview
  * Clear tap/click area

### Individual Parish View
- Large header image
- Visit status banner
  * Not Visited: "You haven't visited [Parish Name] yet!"
  * Visited: "You visited on [Date]"
- Information tabs:
  1. Overview
     * Brief description
     * Contact information
     * Address with map
  2. Mass Schedule
     * Organized by day
     * Special masses highlighted
  3. History
     * Parish founding
     * Historical highlights
     * Photo gallery
  4. Visit Information
     * QR code location hints
     * Parking details
     * Accessibility information

### Visual Indicators
- Clear color-coding:
  * Visited parishes: Diocese brand color
  * Unvisited parishes: Neutral/gray
- Icons:
  * Checkmark for visited
  * Clock for "yet to visit"
  * Special event indicator
- Interactive elements:
  * Hover states
  * Touch feedback
  * Loading states


### Achievement System
- Modern medallion design
- Progress tracking bars
- Unlock requirements
- Share options (with privacy controls)
- Achievement categories:
  * First Visit
  * Multiple Visits
  * Special Events
  * Seasonal Achievements

## Interaction Patterns
- Clear call-to-action buttons
- Intuitive QR code scanning flow
- Confirmation dialogs
- Success/error notifications
- Loading states
- Pull-to-refresh
- Infinite scroll for long lists

## Visual Design Elements
- Diocese brand colors
- Religious iconography
- Modern medallion achievements
- High contrast for readability
- Consistent spacing
- Clear visual hierarchy
- Responsive grid system

## Support & Help
- Contextual help buttons
- FAQ section
- Interactive tutorials
- Contact support form
- System status indicators
- Error handling messages

## Administrative Interface
- Secure login area
- Dashboard with key metrics
- Parish management tools
- QR code generation interface
- Report generation
- User management
- Content management system

## Accessibility Features
- WCAG 2.1 AA compliance
- Screen reader optimization
- Keyboard navigation
- High contrast mode
- Text scaling
- Alternative text
- Focus indicators
- Skip links

## Responsive Design
- Mobile-first approach
- Desktop enhancements
- Tablet optimization
- Touch-friendly interfaces
- Adaptive layouts