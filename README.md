# LearnMate-AI

## Overview

LearnMate-AI is an interactive command-line tool designed to generate personalized learning roadmaps. Based on your specified interests and current skill level, it provides a structured path of topics and explanations to guide your learning journey. The application fetches its course data directly from IBM Cloud Object Storage.

## Features

*   **Personalized Learning Roadmaps:** Get a curated list of topics for any subject in the database.
*   **Skill Level Customization:** Tailor the roadmap for your experience level (Beginner, Intermediate, Advanced).
*   **Interactive CLI:** A simple and user-friendly command-line interface for easy navigation.
*   **Intelligent Suggestions:** If a topic isn't found, the tool suggests the closest available matches.
*   **Cloud-Integrated:** Loads the latest course dataset directly from IBM Cloud Object Storage.

## How It Works

1.  **Data Loading:** The application initiates by loading a course dataset from IBM Cloud Object Storage.
2.  **User Input:** It prompts you to enter the topic you wish to learn (e.g., "UI/UX Design") and your current skill level.
3.  **Roadmap Generation:** The script filters the dataset based on your input and generates a step-by-step roadmap.
4.  **Display Results:** The roadmap is displayed in the console, listing key concepts and their brief explanations.
5.  **Continuous Learning:** After viewing a roadmap, you can press Enter to explore a new topic or type `stop` to exit.

## Getting Started

### Prerequisites

To run this notebook, you need the following Python libraries. You can install them using `pip`:

```bash
pip install pandas ibm-boto3
```

### Running the Application

1.  Clone this repository to your local machine.
2.  Open the `LearnMate AI.ipynb` file in a Jupyter environment such as Jupyter Notebook, JupyterLab, or Google Colab.
3.  Run the cells sequentially.
4.  The interactive prompt will appear in the output of the final cell. Follow the on-screen instructions to generate your first roadmap.

**Example Interaction:**

```
👋 Welcome to LearnMate!
Type 'stop' or 'bye' anytime to exit.

🎯 What are you interested in learning? (e.g., UI/UX Design, Cybersecurity): UI/UX Design
⭐ Select your skill level (Beginner / Intermediate / Advanced): Beginner

📘 Your Beginner Roadmap for: UI/UX Design

1. User Research — Understanding user behaviors, needs, and motivations through observation techniques, task analysis, and other feedback methodologies.
2. Wireframing — A low-fidelity, simplified outline of your product's layout and structure.
3. Prototyping — Creating an interactive, high-fidelity model that mimics the final user interface.
...

🔁 Press Enter to explore another track...
