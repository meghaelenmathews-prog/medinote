# [] 🎯

## Basic Details

**Team Name:** [SAVAGE SISTERS]

### Team Members
- Member 1: [Megha Elen Mathews] - [Viswajothi College of Engineering and Technology]
- Member 2: [Haniya Shahul] - [Viswajothi College of Engineering and Technology]

### Hosted Project Link
[ https://meghaelenmathews-prog.github.io/medinote/]

---

## Project Description

[Medinote is an intelligent, web-based medicine guide application designed to help users quickly find information about medications, symptoms, and health-related queries. Built with a modern, responsive UI, it provides an intuitive interface for accessing medical information with a beautiful gradient design and glass-morphism effects.]

---

## The Problem Statement

[Medinote solves the difficulty patients and caregivers face finding reliable, easy-to-understand medication information. It consolidates curated drug data (dosage, interactions, side effects) and a symptom checker into a searchable, mobile-friendly interface — including offline access — so users can make safer, faster decisions about medicines.]

---

## The Solution

We provide a curated, searchable medicine database combined with a symptom-checker and interaction checker so users can quickly find reliable drug information. The UI uses a fast, mobile-first design with intelligent search, filters, and clear dosage and interaction displays to reduce confusion. Offline caching and local storage enable access without network connectivity; data updates are handled via a verified update pipeline. Safety features include interaction alerts, contraindication warnings, and links to evidence-backed sources. The system integrates optional APIs for drug data, supports personalization (preferences, reminders), and follows accessibility and privacy best practices.



---

## Technical Details

### Technologies/Components Used

#### For Software:

**Languages used:** HTML, CSS, JavaScript

**Frameworks used:** Vanilla JavaScript (no frontend framework)

**Libraries used:** Google Fonts (Poppins); no external JavaScript libraries (uses local JSON/localStorage)

**Tools used:** VS Code, Git, GitHub Pages (hosting), Live Server (local development)

#### For Hardware:

**Main components:** [List main components]

**Specifications:** [Technical specifications]

**Tools required:** [List tools needed]

---

## ✨ Features

List the key features of your project:

- **Smart Medicine Search:** Fast fuzzy search across medicine names, indications, and brands.
- **Symptom Checker:** Guided symptom input with suggested conditions and next-steps.
- **Drug Interaction Alerts:** Automatic warnings for dangerous interactions and contraindications.
- **Dosage & Administration Guides:** Clear dosing, age/weight considerations, and route of administration.
- **Personalized Reminders:** Medication schedules, push/notification reminders, and adherence tracking.
- **Offline Access & Caching:** Local storage caching for access without network connectivity and sync on reconnect.
- **Favorites & Search History:** Bookmark medicines, save notes, and view recent searches.
- **Responsive, Accessible UI:** Mobile-first design, dark mode, and basic WCAG accessibility considerations.
- **Evidence Links & Sources:** Links to trusted medical references and citations for each entry.
- **Export & Print:** Export medicine lists or print patient-friendly summaries (PDF/print-ready).

---

## Implementation

### For Software:

#### Installation

[Installation commands - e.g., npm install, pip install -r requirements.txt]

#### Run

[Run commands - e.g., npm start, python app.py]

### For Hardware:

#### Components Required

[List all components needed with specifications]

#### Circuit Setup

[Explain how to set up the circuit]

---

## Project Documentation

### For Software:

#### Screenshots

![Screenshot1](/screenshot1) 
*Add caption explaining what this shows*

![Screenshot2](/screebshot2) 
*Add caption explaining what this shows*

![Screenshot3](/screenshot3) 
*Add caption explaining what this shows*

#### Diagrams

**System Architecture:**

[┌─────────────────────────────────────────────────────────┐
│                    Medinote Application                  │
├─────────────────────────────────────────────────────────┤
│                                                           │
│  ┌─────────────────────────────────────────────────┐   │
│  │              User Interface Layer                │   │
│  │  ├─ Header Section                              │   │
│  │  ├─ Search Bar                                  │   │
│  │  ├─ Medicine Database Display                   │   │
│  │  └─ Interactive Components                      │   │
│  └─────────────────────────────────────────────────┘   │
│              ↓                                            │
│  ┌─────────────────────────────────────────────────┐   │
│  │          Business Logic Layer (JavaScript)      │   │
│  │  ├─ Search Algorithm                            │   │
│  │  ├─ Data Filtering                              │   │
│  │  ├─ Event Handlers                              │   │
│  │  └─ DOM Manipulation                            │   │
│  └─────────────────────────────────────────────────┘   │
│              ↓                                            │
│  ┌─────────────────────────────────────────────────┐   │
│  │         Data Layer (Local Storage/JSON)         │   │
│  │  ├─ Medicine Database                           │   │
│  │  ├─ User Preferences                            │   │
│  │  └─ Cache Data                                  │   │
│  └─────────────────────────────────────────────────┘   │
│              ↓                                            │
│  ┌─────────────────────────────────────────────────┐   │
│  │        Presentation Layer (CSS/HTML)            │   │
│  │  ├─ Styles & Animations                         │   │
│  │  ├─ Responsive Layout                           │   │
│  │  └─ Visual Effects                              │   │
│  └─────────────────────────────────────────────────┘   │
│                                                           │
└─────────────────────────────────────────────────────────┘] 
*Explain your system architecture - components, data flow, tech stack interaction*

**Application Workflow:**

- **Landing & Search:** User opens the app and sees a prominent search bar and quick links (Symptom Checker, Favorites). As the user types, the frontend filters the local medicines dataset (JSON) and displays ranked results with key metadata.

- **Medicine Detail Flow:** Selecting a medicine opens the detail view showing indications, dosage, side effects, interactions, and evidence links. The UI highlights warnings and shows alternative options where applicable.

- **Interaction Checking:** When the user adds medicines to a temporary list or to their profile, the app runs a client-side interaction check (comparing active ingredients and contraindications) and displays alerts with severity and suggested actions.

- **Symptom Checker Flow:** The guided symptom-checker prompts for symptoms and basic context (age, duration). It returns probable conditions, suggested next steps (self-care, seek medical help), and related medicines to review.

- **Personalization & Reminders:** Users can save favorites, set medication reminders, and store basic preferences in `localStorage`. Reminders use the browser Notification API (with permission) or rely on scheduled local reminders when supported.

- **Offline & Sync:** The app caches core assets and the medicines JSON for offline use. On reconnect, it checks a hosted data file for updates and merges changes while preserving local user data.

- **Export / Print:** Users can export or print patient-friendly medicine summaries (PDF/print-ready) from the detail or favorites view.

- **Admin / Data Update:** Maintainers update the source JSON/data in the repo; a simple CI or manual deploy updates the hosted data used for sync (e.g., via GitHub Pages).

- **Privacy & Safety:** Personal data (favorites, reminders) is stored locally by default. Any optional cloud sync is opt-in and uses secure authenticated APIs; sensitive actions show clear safety warnings and source citations.

---

## Additional Documentation

### For Web Projects with Backend:

#### API Documentation

**Base URL:** `https://api.yourproject.com`

##### Endpoints

**GET /api/medicines**

- Description: Search medicines and return paginated results. Supports searching by name, indication, or active ingredient.
- Query parameters:
  - `q` (string, optional): Search query (medicine name, indication, or ingredient).
  - `page` (integer, optional): Page number (default: 1).
  - `limit` (integer, optional): Items per page (default: 20).
- Response:
  ```json
  {
    "status": "success",
    "data": {
      "total": 123,
      "page": 1,
      "limit": 20,
      "results": [
        {
          "id": "paracetamol_500",
          "name": "Paracetamol 500mg",
          "active_ingredient": "Paracetamol",
          "indications": ["Fever", "Pain"],
          "dosage": "500mg every 4-6 hours; max 4g/day"
        }
      ]
    }
  }
  ```

**POST /api/endpoint**

- Description: [What it does]
- Request Body:
  ```json
  {
    "field1": "value1",
    "field2": "value2"
  }
  ```
- Response:
  ```json
  {
    "status": "success",
    "message": "Operation completed"
  }
  ```

[Add more endpoints as needed...]



## AI Tools Used (Optional - For Transparency Bonus)

If you used AI tools during development, document them here for transparency:

**Tool Used:** [e.g., GitHub Copilot, v0.dev, Cursor, ChatGPT, Claude]

**Purpose:** [What you used it for]
- Example: "Generated boilerplate React components"
- Example: "Debugging assistance for async functions"
- Example: "Code review and optimization suggestions"

**Key Prompts Used:**

- "Create a REST API endpoint for user authentication"
- "Debug this async function that's causing race conditions"
- "Optimize this database query for better performance"

**Percentage of AI-generated code:** [Approximately X%]

**Human Contributions:**

- Architecture design and planning
- Custom business logic implementation
- Integration and testing
- UI/UX design decisions

*Note: Proper documentation of AI usage demonstrates transparency and earns bonus points in evaluation!*

---

## Team Contributions

- **[Name 1]:** [Specific contributions - e.g., Frontend development, API integration, etc.]
- **[Name 2]:** [Specific contributions - e.g., Backend development, Database design, etc.]
- **[Name 3]:** [Specific contributions - e.g., UI/UX design, Testing, Documentation, etc.]

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.

### Common License Options:

- **MIT License** (Permissive, widely used)
- **Apache 2.0** (Permissive with patent grant)
- **GPL v3** (Copyleft, requires derivative works to be open source)

---

Made with ❤️ at TinkerHub

