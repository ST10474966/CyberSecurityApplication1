 CyberGuard - Cybersecurity Awareness Chatbot

Project Overview

CyberGuard is a Windows Presentation Foundation (WPF) application developed in C# using Visual Studio. The application is designed to educate users about cybersecurity by providing interactive conversations, quizzes, reminders, and cybersecurity awareness tips.

The chatbot helps users learn about common cyber threats such as phishing, malware, ransomware, password security, and online privacy while promoting safe online practices.


 Features

* Interactive cybersecurity chatbot
* Cybersecurity quiz with score tracking
* Activity log to record user interactions
* SQL Server database integration
* Task reminder management
* Random cybersecurity tips
* Password security advice
* Sound effects during application startup
* User memory for personalized responses
* Modern WPF graphical user interface

---

## Technologies Used

* C#
* .NET WPF
* Visual Studio 2022
* SQL Server
* Microsoft.Data.SqlClient
* System.Speech.Synthesis
* Git & GitHub

---

## Project Structure

```
CyberSecurityApplication
│
├── MainWindow.xaml
├── MainWindow.xaml.cs
├── ActivityLogEntry.cs
├── QuizQuestion.cs
├── App.xaml
├── App.xaml.cs
├── Assets
│   └── greeting.wav
└── README.md
```

---

## Database

The application uses SQL Server.

Database Name:

```
CyberSecurityDB
```

Example connection string:

```csharp
string connectionString =
@"Server=localhost;
Database=CyberSecurityDB;
Trusted_Connection=True;
TrustServerCertificate=True;";
```

Example Tasks table:

```sql
CREATE TABLE Tasks
(
    Id INT IDENTITY(1,1) PRIMARY KEY,
    Title NVARCHAR(100),
    Description NVARCHAR(255),
    ReminderDate DATETIME,
    Completed BIT DEFAULT 0
);
```

---

## Installation

1. Clone the repository.

```
git clone https://github.com/YourUsername/CyberSecurityApplication.git
```

2. Open the solution in Visual Studio 2022.

3. Restore NuGet packages.

4. Create the SQL Server database.

5. Update the connection string if required.

6. Build and run the project.

---

## How to Use

1. Launch the application.
2. Enter your name.
3. Ask cybersecurity-related questions.
4. Type **quiz** to begin the cybersecurity quiz.
5. Create reminders by typing:

* update my password
* update my profile
* learn about cybersecurity

6. View activity history using the Activity Log button.

---

## Sample Questions

* What is phishing?
* What is malware?
* Tell me about passwords.
* Give me a cybersecurity tip.
* What is ransomware?
* What is a VPN?
* How can I protect my privacy?

---

## Future Improvements

* Speech recognition
* Text-to-speech responses
* User login system
* Quiz timer
* Difficulty levels
* Dashboard with statistics
* Dark/Light mode
* Cloud database support

---

## Author

**Name:** PFUMELANI

Course Project – Cybersecurity Awareness Chatbot

---

## License

This project was developed for educational purposes and may be modified or extended for learning and research.
