# joann-bot: The Social Engineering Responder

The **joann-bot** is a lightweight, single-file web application designed to help users quickly assess and respond to a suspicious communication (email, text, phone call, etc.). It guides the user through a simple decision tree based on common social engineering tactics (urgency, emotional appeals, red flags) to provide a clear risk assessment and recommended actions, including simulated reporting procedures.

---

## Features

* **Guided Decision Flow:** A step-by-step interactive questionnaire covering the most critical indicators of a social engineering attack (e.g., urgency, request for sensitive data, common red flags).
* **Clear Risk Assessment:** Provides immediate feedback classifying the scenario into clear risk levels: **Critical Risk**, **High Risk**, **Moderate Risk (Verification Needed)**, or **Likely Safe**.
* **Actionable Advice:** Every conclusion node gives specific, non-technical advice on how to proceed, focusing on the "Stop, Verify, Report" methodology.
* **Simulated Reporting:** Includes a button to simulate reporting the incident to a security team, reinforcing the procedural step required in a corporate environment.
* **Fully Responsive:** Built with Tailwind CSS for optimal viewing on both mobile devices and desktops.

---

## Technology Stack

* **HTML5:** Structure of the application.
* **JavaScript (Vanilla):** Powers the decision tree logic, navigation, and state management.
* **Tailwind CSS (CDN):** Used for all modern, responsive styling and aesthetics. No separate CSS file is required.

---

## Decision Tree Flow (Simplified)

The application models a common security workflow:

1.  **Start:** Is the communication **unexpected**?
    * *No ->* LIKELY SAFE.
    * *Yes ->* Proceed to check for **Urgency**.
2.  **Urgency Check:** Is there high pressure or strong emotional appeal?
    * *Yes ->* Proceed to check for **Risky Request**.
    * *No ->* Proceed to check for **Red Flags**.
3.  **Risky Request Check:** Does it ask for a password, money transfer, or file download?
    * *Yes ->* **CRITICAL RISK** (Stop and Report).
    * *No ->* Proceed to check for **Red Flags**.
4.  **Red Flag Check:** Are there typos, bad grammar, or strange sender details?
    * *Yes ->* **HIGH RISK** (Verify independently and Report).
    * *No ->* **MODERATE RISK** (Independent Verification Needed).

---

## Contribute and Make joann-bot Better!

This project is meant to be a simple, educational tool, and we strongly encourage you to help us expand and improve it!

**How can you contribute?**

* **Expand the Decision Tree:** Add more detailed nodes for specific attack types (e.g., Vishing, Smishing, Baiting).
* **Improve Styling:** Enhance the user interface and mobile responsiveness.
* **Translate:** Add support for other languages.

Feel free to fork the repository, make your changes, and submit a pull request. Every improvement helps users stay safer online!
