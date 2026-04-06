# Ai-tool-for-early-stage-dementia-detection-
# CogniGuard - Early Dementia Risk Detection

CogniGuard is an AI-assisted cognitive assessment tool designed to identify early signs of dementia risk through a structured questionnaire. It provides users with an instant risk assessment and a personalized 15-day cognitive recovery plan.

## 🔹 Features

- **Home Page**: Introduction to cognitive health and assessment.
- **User Input**: Securely capture user name before assessment.
- **Assessment**: 15 evidence-based cognitive and memory questions with a progress bar.
- **Instant Results**: Score calculation and risk level categorization (Unlikely, Mild Concern, Likely).
- **PDF Report**: Downloadable report including name, score, result, and recovery plan.
- **15-Day Recovery Plan**: Daily brain exercises, physical activities, diet tips, and sleep hygiene.
- **Medical Disclaimer**: Clear communication that the tool is for informational purposes only.

## 🔹 Tech Stack

- **Frontend**: React.js, Tailwind CSS, Lucide React, Motion (framer-motion).
- **Backend**: Node.js with Express.js (Vite middleware for development).
- **Database**: Firebase Firestore (NoSQL).
- **PDF Generation**: jsPDF, jsPDF-autotable.

## 🔹 Project Structure

```text
/
├── server.ts           # Express server entry point
├── src/
│   ├── components/     # React components (Home, Assessment, Result, etc.)
│   ├── lib/            # Firebase and utility functions
│   ├── utils/          # PDF generation logic
│   ├── types.ts        # TypeScript interfaces
│   ├── constants.ts    # Questions and recovery plan data
│   ├── App.tsx         # Routing and main app structure
│   └── main.tsx        # React entry point
├── firestore.rules     # Security rules for database
└── firebase-blueprint.json # Database structure definition
```

## 🔹 Setup & Run Instructions

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Local Setup
1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd react-example
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Environment Variables**:
   Create a `.env` file in the root directory and add your Firebase credentials (if not using the auto-injected ones).
   ```env
   GEMINI_API_KEY=your_api_key
   ```

4. **Run the application**:
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:3000`.

5. **Build for production**:
   ```bash
   npm run build
   npm start
   ```

## 🔹 Medical Disclaimer
CogniGuard is not a medical diagnosis. The results provided are based on self-reported symptoms and should be discussed with a qualified healthcare professional.

## 🔹 License
This project is licensed under the Apache-2.0 License.
