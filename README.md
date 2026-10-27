# MyAccountApp - Mobile Application Development Practical 04

This repository contains the completed code and solutions for **Practical Tutorial 04: Data Transfer Between Screens and Form Handling**, carried out as part of the Mobile Application Development course at the Department of Statistics & Computer Science, University of Kelaniya.

## 📱 Project Overview
`MyAccountApp` is a React Native mobile application built using **Expo Router**. It demonstrates form input handling, state management with `useState`, parameter passing between screens, and basic form validation.

### Features Implemented:
1. **Registration Screen (`app/index.js`)**:
   - Captures user inputs including Username, Email, Phone Number, Year of Birth, Password, and Confirm Password using `TextInput` and `useState`.
   - Performs basic form validation to ensure all fields are filled and passwords match.
   - Calculates the user's age dynamically based on the current year.
   - Passes user details and calculated age securely to the review screen using `router.push`.

2. **Review Screen (`app/review.js`)**:
   - Retrieves passed parameters using `useLocalSearchParams`.
   - Displays the user's submitted details in a clean card layout.
   - Implements **Conditional Navigation**: Validates if the calculated age is under 18 and triggers an `Alert` blocking access if they do not meet the age requirement.
   - Allows users to go back and edit their info using `router.back()`.

3. **Success Screen (`app/success.js`)**:
   - Displays a customized welcome greeting using the user's name (`useLocalSearchParams`).
   - Shows a success confirmation message upon completion.

---

## 🛠️ Tech Stack & Tools
* **Framework:** React Native (Expo)
* **Routing:** Expo Router
* **Language:** JavaScript / JSX
* **Development Environment:** VS Code / Expo Go

---

## 🚀 Getting Started & Running the App

1. **Clone the repository:**
   ```bash
   git clone <your-repository-url>
   cd MyAccountApp