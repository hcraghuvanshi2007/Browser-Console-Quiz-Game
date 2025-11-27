# Lab Assignment 4: Browser Console Quiz Game

## 📋 Project Description

A simple **JavaScript quiz game** that runs entirely in the browser console. This project demonstrates core JavaScript concepts including arrays, loops, conditionals, functions, and user input handling. The quiz asks multiple-choice questions via prompts, validates answers, provides immediate feedback, and tracks the user's score.

## 🎯 Objectives

Upon completing this assignment, you will be able to:

1. Use core JavaScript features: arrays, loops, conditionals, and functions
2. Create and manage arrays to store quiz questions and answers
3. Use for loops to iterate through a set of items systematically
4. Organize code using functions for reusability and clarity
5. Collect user input with `prompt()` and display output with `alert()`
6. Apply string methods (`toLowerCase()`, `trim()`) for accurate input validation
7. Implement conditional statements (if-else) to handle different outcomes
8. Track user performance with a score counter variable
9. Combine loops, conditionals, and functions in a practical application

## 🚀 Features

- ✅ **5+ Quiz Questions**: Comprehensive set of questions with correct answers
- ✅ **User Input Validation**: Uses `toLowerCase()` and `trim()` for case-insensitive, space-tolerant comparison
- ✅ **Immediate Feedback**: Shows correct/incorrect messages after each answer
- ✅ **Score Tracking**: Maintains and displays final score out of total questions
- ✅ **Browser Console Execution**: Runs entirely in the console with no HTML/DOM manipulation required
- ✅ **Clean Code Structure**: Well-organized with arrays, functions, and logical flow

## 📁 File Structure

```
Lab-Assignment-4/
├── 1.html           # Main JavaScript file with quiz logic
└── README.md         # Project documentation (this file)
```

## 💻 How to Use

### Step 1: Open Browser Console
- Press **F12** on your keyboard, or
- Right-click → Select **Inspect** → Go to **Console** tab

### Step 2: Paste the Code
- Copy all code from `quiz.js`
- Paste it into the browser console

### Step 3: Press Enter
- The quiz will start automatically
- A prompt will appear with the first question

### Step 4: Answer Questions
- Type your answer in the prompt box
- Click **OK** to submit or **Cancel** to quit

### Step 5: View Feedback
- After each answer, an alert shows if you're correct or incorrect
- Incorrect answers display the correct answer for learning

### Step 6: Check Final Score
- After all questions, an alert displays your total score

## 📝 Code Structure

### 1. **Quiz Questions Array**
```javascript
const quizQuestions = [
  { question: "...", answer: "..." },
  { question: "...", answer: "..." },
  // ... more questions
];
```
- Stores questions and answers as objects in an array
- Easy to add or modify questions

### 2. **runQuiz() Function**
- Initializes score counter
- Loops through all questions
- Handles user input with prompt()
- Validates and compares answers
- Provides feedback with alert()
- Displays final score

### 3. **Input Normalization**
```javascript
const normalizedAnswer = userAnswer.toLowerCase().trim();
```
- Converts input to lowercase for case-insensitive comparison
- Removes extra spaces for accurate matching

### 4. **Answer Comparison**
```javascript
if (normalizedAnswer === correctAnswer) {
  // Correct answer logic
} else {
  // Incorrect answer logic
}
```

## 📊 Sample Output

**Question Prompt:**
```
What is the capital of France?
```

**User enters:** `PARIS` (with extra spaces: ` PARIS `)

**Feedback Alert:**
```
✓ Correct! Your answer: paris
```

**For Incorrect Answer:**
```
User enters: "london"

Alert:
✗ Incorrect! Your answer: london
Correct answer: paris
```

**Final Score Alert:**
```
Quiz Complete!
Your final score: 4 out of 5
```

## 🔧 Technical Details

| Concept | Implementation |
|---------|-----------------|
| **Arrays** | `quizQuestions[]` stores multiple question objects |
| **Objects** | Each question has `question` and `answer` properties |
| **Loops** | `for` loop iterates through all questions |
| **Functions** | `runQuiz()` organizes all quiz logic |
| **Conditionals** | `if-else` statements check correct/incorrect answers |
| **User Input** | `prompt()` collects user responses |
| **Output** | `alert()` displays feedback and final score |
| **String Methods** | `toLowerCase()` and `trim()` normalize input |
| **Variables** | `score` tracks correct answer count |

## ✨ Quiz Questions Included

1. **What is the capital of France?** → Paris
2. **Which planet is closest to the sun?** → Mercury
3. **What is 2 + 2?** → 4
4. **What is the largest ocean on Earth?** → Pacific
5. **How many continents are there?** → 7

## 🎨 Customization Ideas

### Add More Questions
Simply add new objects to the `quizQuestions` array:
```javascript
{
  question: "What is the smallest prime number?",
  answer: "2"
}
```

### Change Difficulty
Modify questions to be easier or harder based on target audience

### Add Multiple Choice
Extend the logic to display multiple choice options along with free text input

### Add Timer
Implement a time limit for each question using `setTimeout()`

### Track High Scores
Use browser `localStorage` to save and display best scores

### Customize Feedback
Add personalized messages or hints for incorrect answers

## 📋 Performance Rubric (5 Marks)

| Criteria | Marks |
|----------|-------|
| Quiz logic using loops and conditionals | 1 |
| Input handling and answer comparison | 1 |
| Score tracking and display | 1 |
| Knowledge of browser console | 1 |
| Overall code readability and structure | 1 |

## 🔍 Testing Checklist

- [ ] Quiz runs in browser console without errors
- [ ] All 5+ questions display correctly via prompts
- [ ] Case-insensitive comparison works (e.g., "Paris", "PARIS", "paris" all accepted)
- [ ] Extra spaces are trimmed (e.g., " paris " accepted)
- [ ] Correct answers show ✓ feedback and increment score
- [ ] Incorrect answers show ✗ feedback with correct answer
- [ ] Final score displays as "X out of Y"
- [ ] Cancel button allows user to exit quiz
- [ ] Code is clean, commented, and easy to understand

## 📚 Learning Outcomes Achieved

✅ Core JavaScript features understood and implemented  
✅ Arrays used effectively for data storage  
✅ Loops mastered for iteration  
✅ Functions used for code organization  
✅ User input collection and validation practiced  
✅ String methods applied correctly  
✅ Conditional logic implemented  
✅ Score tracking demonstrated  
✅ Problem-solving skills strengthened  
✅ Browser console proficiency developed  

## 🤝 Submission Guidelines

1. Create a GitHub repository named `Lab-Assignment-4`
2. Push `quiz.js` and `README.md` files
3. Ensure minimum 5 questions with working score display
4. Share the GitHub repository link with faculty
5. Test code in browser console before submission

## 📞 Support & Troubleshooting

**Quiz doesn't start?**
- Make sure you pasted the entire code into the console
- Press Enter after pasting
- Check for any error messages in the console

**Answers not being recognized?**
- The system uses lowercase comparison
- Make sure your answers match exactly (after normalization)
- Extra spaces are automatically trimmed

**Score not updating?**
- Check that each answer is being compared correctly
- Ensure the `score++` increments for correct answers
- Verify the final alert displays the score value



**Created:** November 27, 2025  
**Assignment:** Lab 4 - Browser Console Quiz Game  
**Difficulty Level:** Beginner  
**Technology:** JavaScript (Vanilla, Console-based)  
**Author:** B.Tech CSE Student

## 🎮 Quick Start

1. Open browser console (F12)
2. Copy code from `quiz.js`
3. Paste into console
4. Press Enter
5. Answer all questions
6. View your score!

**Happy Coding! 🚀**
