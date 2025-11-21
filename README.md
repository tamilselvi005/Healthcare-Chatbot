Healthcare Chatbot in Java

A simple rule-based healthcare assistant built using pure Java (no external libraries).
This project simulates a real healthcare chatbot that responds to greetings, symptoms, thanks, farewells, and tablet-related queries.

📌 Project Overview

The Healthcare Chatbot is a console-based Java application designed to:

✔ interact with users
✔ identify different types of messages
✔ provide health-related suggestions
✔ recognize symptoms from input
✔ respond with helpful predefined messages

This chatbot does not replace a doctor. It only provides basic information for learning purposes.

🎯 Features
🔹 1. Greeting Detection

The bot recognizes words like:
hello, hi, hey, howdy, greetings
and replies with a random friendly greeting.

🔹 2. Farewell Detection

Supports farewells such as:
bye, goodbye, see you, take care

🔹 3. Thank-you Response

If users type:
thank, thanks, thank you
the bot returns a polite acknowledgment.

🔹 4. Symptom Checker

This is the core functionality.

The bot contains a dictionary of 50+ symptoms, including:

cough

fever

headache

dizziness

chest pain (marked as serious)

difficulty breathing (urgent alert)

fatigue

rash

back pain

anxiety

depression

stomach pain

period pain

blood pressure issues

blood sugar issues

allergies

insomnia

swelling

many more…

When the chatbot finds a symptom word inside the user's message, it responds with the appropriate health suggestion.

🔹 5. Tablet Information

If a user mentions the word “tablet”, the bot explains the purpose of the tablet name given during object creation.

Example:
“The MediHealth tablet is used to treat various health conditions.”

🔹 6. Random Default Replies

If the chatbot doesn’t understand the message, it returns one of the default messages like:

“I'm sorry, I didn't understand that.”

“Could you please repeat that?”

“I'm still learning!”

🔹 7. Exit Option

Typing exit closes the chatbot professionally.

🧠 How It Works

The chatbot processes input in this order:

Greeting? → Send greeting response

Farewell? → Send goodbye response

Thanks? → Send thank-you response

Contains word “tablet”? → Show tablet info

Matches any known symptom? → Show symptom advice

Else → Show default message

It uses:

HashMap<String, String> → for symptoms

List<String> → for greetings, farewells, thanks, defaults

Random() → to generate varied responses

Scanner → for user input

🛠 Technologies Used

Java (JDK 8+)

No frameworks or external libraries

Object-Oriented Programming (OOP)

Collections Framework (List, Map)

▶️ How to Run

Save both HealthcareChatbot and Main classes in the same directory.

Compile using:

javac Main.java


Run the program:

java Main

📚 Learning Outcomes

By doing this project, you will understand:

✔ Java classes & objects
✔ Constructor usage
✔ HashMaps for key-value storage
✔ Lists for storing multiple responses
✔ User interaction using Scanner
✔ Basic AI chatbot logic
✔ String matching & rule-based NLP

🚀 Future Improvements (Optional Ideas)

You can add:

Machine learning–based symptom prediction

GUI using Java Swing

Web integration using Spring Boot

Full diagnosis reports

Chat history storage
