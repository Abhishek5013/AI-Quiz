# QuizWise: AI-Powered Quiz Platform

Created by **Abhishek Yadav**

QuizWise is an interactive web application that allows users to generate quizzes on any topic using the power of Google's Gemini AI. Users can create accounts, take quizzes, and track their progress over time. The application is built with a modern tech stack and provides a seamless, dynamic user experience.

## Features

- **AI Quiz Generation**: Enter any topic and get a custom quiz generated in seconds.
- **User Authentication**: Secure sign-up and login functionality using Firebase Authentication.
- **Personalized Feedback**: After completing a quiz, receive AI-powered feedback on your performance.
- **Progress Tracking**: View your scores over time with an interactive progress chart.
- **Modern UI**: Clean, responsive interface built with ShadCN UI and Tailwind CSS.

## Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) (with App Router)
- **AI Integration**: [Genkit](https://firebase.google.com/docs/genkit) with Google's Gemini Model
- **Backend & Authentication**: [Firebase](https://firebase.google.com/)
- **UI Components**: [ShadCN UI](https://ui.shadcn.com/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)

---

## Getting Started

Follow these instructions to get the project running on your local machine.

### Prerequisites

- You need [Node.js](https://nodejs.org/) (version 18 or later) installed.
- You need a Google account for Firebase and Gemini.

### 1. Installation

Clone the repository and install the project dependencies using npm:

```bash
npm install
```

### 2. Set Up Environment Variables

This project requires a Google Gemini API key to generate quizzes.

1.  **Get a Gemini API Key**: Visit [Google AI Studio](https://aistudio.google.com/app/apikey) to create and copy your API key.
2.  **Create an Environment File**: In the root of your project, create a file named `.env`.
3.  **Add the Key**: Add the following line to your `.env` file, replacing `YOUR_API_KEY_HERE` with your key.

    ```
    GEMINI_API_KEY=YOUR_API_KEY_HERE
    ```

### 3. Configure Firebase

The application uses Firebase for user authentication. You will need to create a Firebase project and enable Email/Password authentication.

1.  Go to the [Firebase Console](https://console.firebase.google.com/).
2.  Create a new project.
3.  Navigate to **Build > Authentication**.
4.  Select the **Sign-in method** tab.
5.  Click on **Email/Password** and **Enable** it.

### 4. Running the Development Server

Once the installation and configuration are complete, you can start the local development server:

```bash
npm run dev
```

Open [http://localhost:9003](http://localhost:9003) with your browser to see the result.

---

## Deployment

The easiest way to deploy this Next.js application is to use the [Vercel Platform](https://vercel.com/new).

When deploying, remember to add your `GEMINI_API_KEY` as an Environment Variable in your Vercel project settings.
