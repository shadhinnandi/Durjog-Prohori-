# Durjog Prohori

## A coordinated digital platform for disaster awareness, emergency reporting, and response

Durjog Prohori is a full-stack disaster-management platform designed to connect people affected by disasters with the organizations and responders who can help them. It brings alerts, emergency reports, maps, donations, relief coordination, and role-based operations into one accessible system.

The platform is built for fast-moving situations where reliable information, clear ownership, and timely response matter most.

## Highlights

- **Disaster awareness:** Track and present flood, cyclone, fire, earthquake, landslide, tsunami, and other disaster information.
- **Emergency reporting:** Submit site reports and SOS requests with location-aware details for faster assessment.
- **Interactive maps:** Visualize disasters, reports, responders, and operational locations using Leaflet and React Leaflet.
- **Role-based response:** Dedicated workflows for citizens, authorities, firefighters, NGOs, and administrators.
- **Firefighter operations:** Manage firefighter profiles, equipment, assignments, locations, and disaster reports.
- **Authority coordination:** Review incidents, assign response teams, manage reports, and monitor emergency activity.
- **NGO relief support:** Coordinate resources, review reports, and manage donation and relief workflows.
- **Community support:** Connect users with blood donors, donations, support requests, and community communication.
- **Real-time notifications:** Deliver user and operational updates through notification services and Socket.IO communication.
- **Weather and earthquake awareness:** Provide weather information and earthquake notification features for proactive preparation.
- **Accessible experience:** Responsive React interfaces with light/dark theme support and internationalization foundations.

## Platform roles

### Citizens

Citizens can view disaster information, receive alerts, report incidents, use emergency and SOS workflows, explore maps, request support, donate, and access community services.

### Authorities

Authorities can review disaster activity, manage reports, assign firefighters and NGOs, monitor response operations, and coordinate emergency resources.

### Firefighters

Firefighters can manage their profiles and equipment, view assignments, report disaster activity, and share operational location information.

### NGOs

NGOs can manage relief resources, review reports, coordinate support, and participate in donation and emergency-response workflows.

### Administrators

Administrators can manage platform data, users, disaster records, and operational workflows across the system.

## Technology

| Area | Technology |
| --- | --- |
| Frontend | React 18, React Router, React Bootstrap, Tailwind CSS |
| Maps | Leaflet, React Leaflet, React Leaflet Cluster |
| State and UX | Zustand, React Context, React Toastify, i18next |
| Backend | Node.js, Express |
| Database | MongoDB, Mongoose |
| Authentication | JWT and bcrypt |
| Real-time communication | Socket.IO |
| Integrations | Axios, Nodemailer, Firebase |

## Project structure

```text
Durjog_Prohori/
├── client/                 # React web application
│   └── src/
│       ├── components/     # Shared and role-specific UI
│       ├── pages/          # Authority, firefighter, NGO, and user pages
│       ├── context/        # Authentication, language, theme, and role state
│       ├── services/       # Scheduled and external service integrations
│       └── store/          # Client-side state stores
├── models/                 # MongoDB/Mongoose data models
├── routes/                 # Authentication, disaster, report, donation, and role APIs
├── middlewares/            # Authentication and request middleware
├── public/                 # Public server assets
├── scripts/                # Setup, diagnostics, and API utility scripts
├── server.js               # Main Express application
└── package.json            # Project scripts and server dependencies
```

## Getting started

### Prerequisites

- Node.js 18 or later
- npm
- MongoDB, local or hosted

### Installation

```bash
git clone <repository-url>
cd Durjog_Prohori
npm install
cd client
npm install
cd ..
```

Create the required environment configuration for the server and client. Keep credentials and private service keys out of version control. At minimum, configure the MongoDB connection value expected by the server:

```env
MONGO_URI=mongodb://localhost:27017/durjog-prohori
```

### Run the application

Run the API and React client together:

```bash
npm run dev
```

Or run them separately:

```bash
# API server
npm run server

# React client
npm run client
```

Create a production frontend build with:

```bash
npm run build
```

## API areas

The backend is organized around focused route modules, including:

- Authentication and user accounts
- Disaster records and disaster-specific data
- Site reports and SOS reports
- Authority and firefighter operations
- NGO and relief workflows
- Donations and NGO donations
- Support requests and user notifications

## Product vision

Durjog Prohori is more than an incident form or an alert page. It is designed as a shared response layer where:

1. **People can report what is happening.**
2. **The right organization can receive and classify the report.**
3. **Responders can be assigned with location and operational context.**
4. **Communities can contribute support, resources, and information.**
5. **Authorities can coordinate the response from a unified view.**

## Project status

Durjog Prohori is an actively developed academic team project. Features and integrations may continue to evolve as the platform is tested and refined.
