# Temperature Monitoring System (C)

A simple C-based console application that simulates a continuous temperature
monitoring system with alert classification.

This project was built to practice:
- Functions
- Conditional logic
- Input validation
- Loop control in C

---

## 📌 Features

- Accepts real-time temperature input from the user
- Classifies temperature into:
  - NORMAL
  - WARNING
  - CRITICAL
- Handles invalid (non-numeric) input safely
- Allows the user to continue or exit gracefully

---

## 🧠 Temperature Classification Logic

| Temperature Range (°C) | Status                       |
|------------------------|------------------------------|
| ≤ -45                  | CRITICAL (Extreme cold)      |
| -45 to -20             | WARNING (Abnormally cold)    |
| -20 to < 50            | NORMAL                       |
| 50 to < 75             | WARNING (Temperature rising) |
| ≥ 75                   | CRITICAL (Extreme heat)      |

---

## ▶️ How to Run

1. Compile the program using a C compiler:
   ```bash
   gcc main.c -o temperature_monitor
