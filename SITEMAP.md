# Site Map and Navigation Flow

## Visual Navigation Structure

```
                    index.html (redirects to →)
                            ↓
                    landing_page.html
                    (Interactive Desk Scene)
                            ↓
                    ┌───────┴───────┐
                    │               │
            📖 Click Book    🧹 Click Eraser
                    │               │
                    ↓               ↓
                story.html      projects.html
            (The Crossroads)   (Page 12)
                    │
        ┌───────────┼───────────┬───────────┐
        │           │           │           │
        ↓           ↓           ↓           ↓
  projects.html leadership.html leadership- publications.html
    (Page 12)    (Page 28)    profile.html    (Page 45)
                                (Page 35)
```

## Page Details

### Landing Page (`landing_page.html`)
- **Type:** Entry point
- **Navigation:**
  - Book → `story.html`
  - Eraser → `projects.html`
- **Purpose:** Visually engaging entry with narrative setup

### Index (`index.html`)
- **Type:** Redirect page
- **Navigation:** Auto-redirects to `landing_page.html`
- **Purpose:** Catch-all entry point

### Story (`story.html`)
- **Page:** 1
- **Title:** "The Crossroads of Data"
- **Navigation:**
  - → `projects.html` (Data Projects Laboratory)
  - → `leadership.html` (Leadership Chamber)
  - → `leadership-profile.html` (Complete Leadership Profile)
  - → `publications.html` (Publications Archive)
  - ← `landing_page.html` (Return to Cover)
- **Purpose:** Main navigation hub with narrative framing

### Projects (`projects.html`)
- **Page:** 12
- **Title:** "The Data Projects Laboratory"
- **Navigation:**
  - → `leadership.html`
  - → `publications.html`
  - → `story.html` (Return to Crossroads)
- **Content:** Project cards with descriptions, tech stacks, and GitHub links

### Leadership (`leadership.html`)
- **Page:** 28
- **Title:** "The Leadership Chamber"
- **Navigation:**
  - → `projects.html`
  - → `publications.html`
  - → `leadership-profile.html` (Complete Profile button)
  - → `story.html` (Return to Crossroads)
- **Content:** Assessment cards (MBTI, StrengthsFinder, EQ, etc.)

### Leadership Profile (`leadership-profile.html`)
- **Page:** 35
- **Title:** "Complete Leadership Profile"
- **Navigation:** (Check the actual file for navigation)
- **Content:** Comprehensive integration of all assessments

### Publications (`publications.html`)
- **Page:** 45
- **Title:** "The Publications Archive"
- **Navigation:**
  - → `projects.html`
  - → `leadership.html`
  - → `story.html` (Return to Crossroads)
- **Content:** Publication entries, contact information, "The End"

## Quick Reference: Where Each Link Goes

| Current Page | Link Text | Destination |
|-------------|-----------|-------------|
| landing_page | Book area | story.html |
| landing_page | Eraser area | projects.html |
| story | Data Projects | projects.html |
| story | Leadership Chamber | leadership.html |
| story | Leadership Profile | leadership-profile.html |
| story | Publications Archive | publications.html |
| story | Return to Cover | landing_page.html |
| projects | Leadership Skills | leadership.html |
| projects | Publications | publications.html |
| projects | Return to Crossroads | story.html |
| leadership | Data Projects | projects.html |
| leadership | Publications | publications.html |
| leadership | Complete Profile | leadership-profile.html |
| leadership | Return to Crossroads | story.html |
| publications | Data Projects | projects.html |
| publications | Leadership Skills | leadership.html |
| publications | Return to Crossroads | story.html |

## User Journeys

### Journey 1: Full Experience
1. `landing_page.html` → Click Book
2. `story.html` → Read narrative, choose Data Projects
3. `projects.html` → Review projects, go to Leadership
4. `leadership.html` → See assessments, view Complete Profile
5. `leadership-profile.html` → Deep dive into leadership style
6. Return to Crossroads → Go to Publications
7. `publications.html` → Read publications, see contact info

### Journey 2: Quick Access
1. `landing_page.html` → Click Eraser
2. `projects.html` → Directly view projects
3. Navigate to other sections as desired

### Journey 3: Exploration
1. Enter via any page
2. Use bottom navigation to move between sections
3. Return to Crossroads (`story.html`) at any time
4. Jump to any other section from there

## Notes

- All pages are interconnected
- No dead ends - every page has navigation options
- "Return to Crossroads" consistently goes to `story.html`
- Story page serves as central hub for deep exploration
- Projects page can be reached directly via "Skip the Story"
