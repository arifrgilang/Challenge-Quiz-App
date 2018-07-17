# Challenge Quiz App
**The challenge is down below**

This repository consist of a Quiz App. You should finish the challenge. Keep track the time and what you changed inside the files.

## Whats Important Inside
- Function for saving InstanceState (onSaveInstanceState)
- Function that pass data between Activity, and Returning it when user go back
- Overriding Activity cycle function
- Intent, and putting extra value into it
- Animation
- Handle for different API Version
- Log for debugging

## First State of the App [Tue-17-07-2018]

### Model
  - Question has:
    - TextResId (Contain id for question)
    - AnswerTrue (The answer)
    
### View
  - activity_quiz
  - activity_cheat

### Controller
  - QuizActivity has:
    - TextView (Question)
    - 2 Button (True and False)
    - Cheat Button (Intent to CheatActivity
    - 2 Button (Prev and Next)
  
  - CheatActivity has:
    - TextView (Warning text)
    - TextView (Answer for the question)
    - Button (Show Answer Button)
  
The app could handle landscape or portrait situation so you didn't need to worry about activity cycle.

Upon pressed, true false button will execute a toast "Correct" or "Incorrect", howewer if user uses cheat, "Cheating is wrong" will show up instead

If user go to CheatActivity without showing the answer, that doesn't count as cheating

if user cheating, go back to QuizActivity, then hover to another question and back again, the cheat counter is reset (this is bug)

## The Challenge

**1. Preventing Repeat Answer** - You should disable the button once user answer the question

**2. Graded Quiz** - After user finished answering all the question, display a Toast with percentage score of the quiz

**3. Closing Loopholes for cheater** - Handle situation when cheater go could cheat, and change question and then go back to reset the cheat detector.

**4. Reporting the build Version** - Add a text view below the Show Answer button in CheatActivity

**5. Limited Cheats** - Limit the cheat into 3 times. Keep track of the user's cheat occurences, display remaining cheat token, disable cheat button if no token remains.
  
