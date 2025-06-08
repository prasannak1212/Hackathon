QuizCraft Project Documentation

High-Level Solution Overview:
QuizCraft is an interactive quiz web application built for a mini hackathon. The app allows users to select quiz categories, answer multiple-choice questions, and view scores in real-time. It is designed with a focus on engaging UI, efficient state management, and scalable Firebase backend support. The project targets both casual users and educational purposes by offering category-wise knowledge testing and tracking user performance.

How to Run the Project:

Frontend:

Clone the repository.

Navigate to the project directory.

Open index.html directly in a browser or serve using a simple HTTP server:

npx serve .

Ensure Firebase SDK is properly configured with your credentials in the firebase-config.js file.

Backend:
There is no traditional backend server. Firebase handles authentication, database, and hosting.

Firebase Integration Steps:

Go to Firebase Console and create a new project.

Add a web app to the Firebase project.

Copy the Firebase configuration and replace it in your firebase-config.js:

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
firebase.initializeApp(firebaseConfig);

Enable Firebase Authentication (Email/Password or anonymous).

Create Firestore Database with the required collections like quizzes, scores, etc.

Use Firebase Hosting (optional) to deploy.

Repository Link:
GitHub - QuizCraft (Replace with actual link)

Tools/Libraries Used:

Frontend:

HTML, CSS, JavaScript (Vanilla)

Bootstrap (for styling and responsive layout)

Backend / BaaS:

Firebase Authentication

Firebase Firestore (for storing questions, scores)

Firebase Hosting (optional deployment)

Other Tools:

VSCode (development environment)

Git & GitHub (version control)

Deployment / Local Setup Steps:

Local Setup:

Clone the repo:

git clone https://github.com/your-username/quizcraft.git

Navigate to the project folder:

cd quizcraft

Install a live server (if not installed):

npm install -g serve

Run the app locally:

serve .

Firebase Hosting (Optional):

Run firebase login.

Initialize project:

firebase init

Deploy:

firebase deploy

Feel free to update Firebase config and styling to customize the app further.

