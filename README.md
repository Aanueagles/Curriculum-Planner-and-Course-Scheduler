
---

🎓 Curriculum Planner and Course Scheduler

This is a Python-based command-line tool designed for undergraduate students to manage and plan their academic journey. It allows users to create personal schedules, manage course prerequisites, track academic progress, and ensure they are on track for graduation.

---

## 🚀 Features

- ✅ Multi-user login using Matric Number and Password
- ✅ Secure password hashing using SHA-256
- ✅ View all available courses and their prerequisites
- ✅ Add new courses with details like credit hours and prerequisites
- ✅ Build and save personalized semester course schedules
- ✅ Check and enforce prerequisite conditions
- ✅ Track completed credit hours and estimate graduation progress
- ✅ Automatically save each student’s schedule in a personal JSON file
- ✅ JSON-based data storage (no external database required)

---

## 🛠️ Technologies Used

- **Language**: Python 3.x
- **Storage**: JSON files for users, courses, and schedules
- **Security**: `hashlib` for password hashing
- **OS**: Cross-platform (Windows, Linux, macOS)

---

## 🔐 User Authentication

- Users are identified by their **matric number**
- Passwords are **hashed** before saving, ensuring they are not stored in plain text
- Each user's schedule and academic progress is stored separately

---

## 🗂 File Structure

```

├── curriculum\_planner.py         # Main program file
├── courses.json                  # All available courses
├── profiles.json                 # Registered users (hashed passwords)
├── \[MATRIC\_NUMBER]\_schedule.json # Individual user course schedule

````

---

## 💻 How to Run

### 1. Install Python (if not already installed)
Download Python from: https://www.python.org/downloads/

### 2. Clone or Download the Project

```bash
git clone https://github.com/your-username/curriculum-planner.git
cd curriculum-planner
````

### 3. Run the Script

```bash
python curriculum_planner.py
```

---

## 📋 How It Works

### 🧑‍🎓 Student Usage Flow:

1. **Login/Register**
   Enter your matric number and password. If you are new, you’ll be asked to create one.

2. **Main Menu Options**

   ```
   1. View all courses
   2. Add a new course
   3. Plan your schedule
   4. Track credit progress
   5. Exit
   ```

3. **Add Courses**
   You can input course code, title, credit hours, and any prerequisites.

4. **Plan Schedule**
   Pick from available courses and only valid ones (with satisfied prerequisites) will be added.

5. **Track Progress**
   Shows completed credits and how many are left to reach graduation target (usually 120 credits).

---

## 🧪 Example Use Case

1. Matric number: `CSC2023004`
2. Password: `MyStrongPass`
3. Adds 100-level courses: CSC101, MTH101, etc.
4. Builds 1st semester schedule
5. Later, uses “Track progress” to check how many credits are done

---

## 🔧 Future Improvements

* Duplicate course prevention
* GPA calculator
* Graphical User Interface (GUI)
* Web-based version with database
* Admin panel for academic advisors

---

## 🙋 FAQ

**Q: What if a course has prerequisites?**
A: You can only add it to your schedule after completing the prerequisite course(s).

**Q: Are passwords secure?**
A: Yes. They are hashed using `SHA-256` and never stored as plain text.

**Q: Can multiple students use it?**
A: Yes, each student is identified by their unique matric number and has a private file.

---

## 📄 License

This project is open-source and free to use for educational purposes.

---

## 👨‍💻 Author

Developed by Oyedepo Joseph Aanuoluwapo.
Feel free to contribute, fork, or improve!

