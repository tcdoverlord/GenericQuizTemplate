# Generic Quiz Template

[![Generic Quiz Template Demo](https://github.com/tcdoverlord/GenericQuizTemplate/blob/main/GenericQuiz_Hero_Vid.gif)](https://github.com/tcdoverlord/GenericQuizTemplate/blob/main/GenericQuiz_Hero_Vid.gif)

A reusable, responsive HTML and JavaScript quiz template for creating interactive quizzes without frameworks, libraries, or external dependencies.

The template includes built-in support for single-answer questions, multiple-answer questions, hints, explanations, scoring, grading, quiz reset, and light/dark mode.

## Features

- **Single-answer questions** using radio buttons
- **Multiple-answer questions** using checkboxes
- **Required answer selection**
- Detects incomplete multiple-answer questions
- Tells the user when additional choices are required
- Prevents partially answered multi-answer questions from being graded as simply incorrect
- Displays **Correct** or **Incorrect** feedback
- Provides explanations after submitting answers
- Optional hints for individual questions
- Automatic score calculation
- Displays correct answers, missed answers, percentage, and letter grade
- Light and dark mode with saved theme preference
- Responsive design for desktop and mobile devices
- Reset Quiz button
- No frameworks or external JavaScript libraries
- No build system required
- Runs directly in a web browser

## How to Use

### 1. Clone or download the repository

```bash
git clone https://github.com/your-username/html-quiz-template.git
```

Or download the repository as a ZIP file from GitHub.

### 2. Open the template

Open `index.html` in any modern web browser.

No installation or build process is required.

## Creating Your Own Quiz

The quiz questions are stored in the `questions` array inside `index.html`.

Replace the example questions with your own.

### Single-Answer Question

Use one item in the `answer` array:

```javascript
{
  question: "What is 2 + 2?",
  options: ["3", "4", "5", "6"],
  answer: ["4"],
  explanation: "2 + 2 equals 4.",
  hint: "Think about adding two groups of two."
}
```

The template automatically uses radio buttons when only one answer is required.

### Multiple-Answer Question

Use multiple items in the `answer` array:

```javascript
{
  question: "Select all prime numbers. (Select TWO.)",
  options: ["4", "5", "6", "7"],
  answer: ["5", "7"],
  explanation: "5 and 7 are prime numbers.",
  hint: "A prime number greater than 1 has exactly two positive divisors."
}
```

The template automatically uses checkboxes when multiple answers are required.

The number of items in the `answer` array determines how many choices the user must select.

## Multiple-Answer Validation

If a question requires two answers and the user selects only one, the template provides a clear message:

> This question requires 2 choices. Please select 1 more choice to continue.

This helps prevent partially answered questions from being incorrectly treated as completed.

## Hints

Questions can optionally include a `hint`:

```javascript
hint: "Think about adding two groups of two."
```

The user can reveal or hide the hint when needed.

## Explanations

Each question can include an explanation:

```javascript
explanation: "2 + 2 equals 4."
```

Explanations are displayed with the answer feedback after submission.

## Scoring

After the quiz is submitted, the template calculates:

- Correct answers
- Missed answers
- Percentage
- Letter grade

The current grading scale is:

| Percentage | Grade |
|---|---|
| 90%–100% | A |
| 80%–89% | B |
| 70%–79% | C |
| 60%–69% | D |
| Below 60% | F |

## Light and Dark Mode

The template includes a built-in light/dark mode toggle.

The selected theme is saved in the browser using `localStorage`.

If no preference has been saved, the template can use the user's system color preference.

## Customization

You can customize:

- Quiz title
- Subtitle
- Questions
- Answer choices
- Correct answers
- Hints
- Explanations
- Colors
- Layout
- Grading scale
- Button text
- Styling

Most quiz customization can be done by editing the `questions` array.

## Project Structure

```text
html-quiz-template/
├── index.html
└── README.md
```

## No Dependencies

This project uses:

- HTML
- CSS
- Vanilla JavaScript

There are no frameworks, package managers, build tools, or external libraries required.

Simply open `index.html` in a browser.

## Example Questions

The repository includes example questions so the template can be tested immediately after downloading.

Replace those examples with your own questions without changing the quiz engine.

## License

Feel free to modify and use this template for your own projects.

Contributions, improvements, and suggestions are welcome.
