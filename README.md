# -Simple-Math-Quiz-App

🧠 Simple Math Quiz App (Android - Java)
A basic Android app built using Java and XML that helps users practice simple addition and multiplication problems. It also keeps track of correct and wrong answers.


**📲 Features**

Random math questions (+ or ×)

Score tracking: ✅ Correct / ❌ Wrong

Input answer and submit

Result feedback (Correct / Wrong)

Auto-generate new question after each answer


**🛠 Tech Stack**

Language: Java

IDE: Android Studio

Layout: XML with LinearLayout

Min SDK: API 21 (Lollipop) or above




**🧑‍💻 Object-Oriented Programming (OOP) Concepts Used**

**Encapsulation:** All variables and methods are organized inside the MainActivity class.

**Abstraction:** Complex tasks like checking answers and generating questions are handled in separate methods (checkAnswer(), generateQuestion(), updateCounts()).

**Modularity:** Logic is broken into clean, reusable functions.

**Class Usage:** MainActivity extends AppCompatActivity, showing class inheritance in action.







**📁 Files Included**

MainActivity.java – Java class with logic for the app

activity_main.xml – XML layout for UI




**🔄 How it Works**

A random question (e.g., 6 + 3 = ? or 7 * 2 = ?) is generated.

User enters an answer in the input field.

On submit:

✅ If correct: "Correct! 🎉" + increment correct score

❌ If wrong: "Wrong! Try again." + increment wrong score

A new question is shown immediately.



**💡 Code Highlights**

Random random = new Random();
num1 = random.nextInt(10) + 1;
num2 = random.nextInt(10) + 1;
correctAnswer = isAddition ? num1 + num2 : num1 * num2;


**Answer Check Logic:**

if (answer == correctAnswer) {
    tvResult.setText("Correct! 🎉");
    correctAnswers++;
} else {
    tvResult.setText("Wrong! Try again.");
    wrongAnswers++;
}




