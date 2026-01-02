# HCI News Reading Study

## About

This project is a **Human-Computer Interaction (HCI)** research study developed for the **CS449/549 HCI course**. The goal is to investigate how user interface design affects reading behavior and comprehension on news websites.

The study uses an **A/B testing methodology** to compare two different UI approaches: a traditional cluttered design versus a focus-optimized design that applies HCI principles to reduce cognitive load and improve user experience.

## Purpose

This study investigates how different UI design approaches affect:
- **Reading time** - How long users spend reading articles
- **Scroll depth** - How much of the article users read
- **Comprehension** - How well users understand the content
- **Perceived focus** - How focused users feel while reading
- **Distraction clicks** - How often users click on non-article elements

## HCI Principles Applied

The study tests several key HCI concepts:
- **Cognitive Load Theory** - Reducing visual clutter to improve focus
- **Hick's Law** - Limiting choices to reduce decision time
- **Progressive Disclosure** - Showing information only when needed
- **Visual Hierarchy** - Guiding attention through design
- **Feedback & Affordances** - Progress indicators and clear controls

## UI Designs Compared

### UI-A: Classic Design (Control)
- Traditional news website layout with sidebar
- Advertisements (inline and sidebar)
- Related articles section
- Trending news widgets
- Multiple visual distractions

### UI-B: Focus Frame Design (Treatment)
Applies HCI principles to reduce cognitive load:
- **Single-column layout** - No sidebar distractions
- **Progress indicator** - Shows reading progress
- **Focus Mode** - Dims everything except the article
- **Summary box** - Key points at the start
- **Section markers** - Visual reading milestones
- **Text controls** - Adjustable font size and line spacing
- **Motivation popups** - Encouragement at 50%, 75%, 90% progress

## Study Flow

1. **Landing** - Study introduction
2. **Consent** - Participant agreement
3. **Profile** - Demographics (age, gender, occupation, interests)
4. **Scenario 1** - Read article on first UI design
5. **Survey 1** - Comprehension question + ratings
6. **Scenario 2** - Read article on second UI design
7. **Survey 2** - Comprehension question + ratings
8. **Thank You** - Completion code

## Data Collected

Each session records:
- Participant demographics
- UI version (A or B)
- Article topic
- Reading time (seconds)
- Maximum scroll depth (%)
- Distraction clicks (UI-A only)
- Focus mode usage (UI-B only)
- Comprehension score (correct/incorrect)
- Perceived focus rating (1-7)
- Perceived readability rating (1-7)

## Tech Stack

- Pure HTML/CSS/JavaScript (no frameworks)
- Firebase Realtime Database for data storage
- LocalStorage as backup
- CSS conic-gradient for donut charts

## Files Structure

```
├── index.html        # Redirect to landing
├── landing.html      # Study introduction
├── consent.html      # Participant consent form
├── profile.html      # Demographics form
├── scenario.html     # Scenario start page
├── feed-a.html       # UI-A news feed
├── feed-b.html       # UI-B news feed
├── reader-a.html     # UI-A article reader
├── reader-b.html     # UI-B article reader
├── survey.html       # Post-reading survey
├── thankyou.html     # Completion page
├── results.html      # Data visualization dashboard
├── styles.css        # Shared styles
└── tracking.js       # Firebase data handling
```

## Results Dashboard

Access `results.html` to view:
- Participant demographics charts
- UI-A vs UI-B comparison
- Comprehension scores by UI version
- Reading time comparison
- Export data as JSON/CSV

## Running Locally

Simply open `index.html` in a browser, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve
```

## Within-Subject Design

Each participant experiences both UI designs (counterbalanced order: AB or BA) to control for individual differences.

## License

Academic use only. Created for CS449/549 HCI course.
