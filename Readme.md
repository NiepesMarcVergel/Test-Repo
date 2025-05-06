# 📖 Digital Diary - C# Console Application

## ⚙ Project Description

**Digital Diary** is a modular, console-based C# application that allows users to maintain a personal diary. Users can:
- Write new diary entries
- View all saved entries
- Search entries by date

Entries are stored in a local text file (`diary.txt`) using file handling techniques, ensuring that all data will be saved and can be used  across sessions. This project demonstrates a clean implementation of object-oriented programming (OOP) principles in C#.

## 🔧 Features

- **Write Entries:** Add new entries with timestamped logs.
- **View Entries:** Display all past entries saved in the diary.
- **Search by Date:** Find specific entries using a YYYY-MM-DD formatted date.
- **File Persistence:** All data is stored in a text file using `StreamWriter` and `File.ReadAllText`.
- **Error Handling.** Ensures basic error handling to manage invalid inputs and missing files.


## 🕹 OOP Principles Used

- **Encapsulation:** The Diary class encapsulates the filePath field and related operations (WriteEntry, ViewAllEntries, and SearchByDate) to manage diary entries. The filePath is marked as private readonly, which hides it from external classes and prevents modification, protecting the integrity of the data.

- **Abstraction:** The Diary class provides simple public methods to write, view, and search entries without exposing how those operations interact with the file system. The user of the class doesn’t need to understand file handling to use the diary functionality.

- **Modularity:** Functionality is separated into `Diary.cs` for logic and `Program.cs` for user interaction and flow. The Diary class is a self-contained module for diary management. The Program class is responsible for user interaction and control flow, keeping concerns separate from diary logic.


## 📄 How to Run the Application

1. Open the project in **Visual Studio** or any C#-compatible IDE.
2. Ensure the following files are present:
   - `Program.cs`
   - `Diary.cs`
3. Build the solution.
4. Run the application.
5. Follow the menu to write, view, or search diary entries.

## 📝 File Structure

```
Diary/
├── bin/
│   └── Debug/
│       └── net9.0/
├── obj/
├── Diary.cs
├── Lab 3.csproj
├── Program.cs
├── README.md
└── diary.txt
```

## 🖼 Sample Output

```
Diary Menu:
1. Write a New Entry
2. View All Entries
3. Search Entry by Date
4. Exit
Enter your choice: 1
Enter your diary entry (end with an empty line):
Learning C# is fun, I hope I'll learn more~

Entry saved.

Diary Menu:
1. Write a New Entry
2. View All Entries
3. Search Entry by Date
4. Exit
Enter your choice: 2

All Entries:

Date: 2025-05-01 15:00:00
Learning C# is fun, I hope I'll learn more~
---

Diary Menu:
1. Write a New Entry
2. View All Entries
3. Search Entry by Date
4. Exit
Enter your choice: 3
Enter date to search (YYYY-MM-DD): 2025-05-01

Date: 2025-05-01 15:00:00
Learning C# is fun, I hope I'll learn more~

Diary Menu:
1. Write a New Entry
2. View All Entries
3. Search Entry by Date
4. Exit
Enter your choice: 4
```

## 👥Team Members

- Alcaraz John  
- Bulanadi Sophia Loureine  
- Comia Ian Emmanuel  
- Niepes Marc Vergel  

## 📃 Acknowledgement

Special thanks to our Advance Object-Oriented Programming professor Marie Agdon for guiding us in understanding the C# language and object-oriented programming concepts. We would also like to give our gratitude to all of our supportive classmates and parents that motivate us in making this project come into  a success. They all helped us push further and be able to apply our learning in  real-world scenarios.


