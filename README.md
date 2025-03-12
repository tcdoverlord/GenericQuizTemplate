# Generic Quiz Template

This repository contains a reusable and dynamic quiz template built with HTML and JavaScript. It allows users to create interactive quizzes by simply updating the provided `questions` array.

## How to Use

1. Clone or download the repository:
   ```bash
   git clone https://github.com/your-username/GenericQuizTemplate.git
2.	Open the index.html file in any web browser.
Features
•	Fully dynamic: Add new questions, options, and answers in the questions array within the JavaScript code.
•	Handles single-answer and multiple-choice questions seamlessly.
•	Displays correct/incorrect answers, explanations, and a results summary with percentage and grade.
Example Questions
You can replace the current questions array with your own. Here's an example of what the questions array looks like:
const questions = [
  {
    question: "What is 2 + 2?",
    options: ["3", "4", "5", "6"],
    answer: ["4"],
    explanation: "2 + 2 equals 4."
  },
  {
    question: "Select all prime numbers.",
    options: ["4", "5", "6", "7"],
    answer: ["5", "7"],
    explanation: "Prime numbers are only divisible by 1 and themselves. Here, 5 and 7 are prime."
  }
];
________________________________________
License
Feel free to modify and use this template. Contributions are welcome!
