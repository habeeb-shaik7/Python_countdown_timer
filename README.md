# Python Countdown Timer

A simple **countdown timer built using Python**. The program takes the time in seconds from the user and counts down to zero in `MM:SS` format.

## 📌 Features

* Takes countdown time from the user
* Displays time in **minutes and seconds**
* Updates the timer every second
* Displays a message when the countdown finishes
* Simple and beginner-friendly Python project

## 🛠️ Technologies Used

* **Python**
* `time` module

## 🚀 How It Works

1. The user enters the countdown time in seconds.
2. The program converts the input into an integer.
3. `divmod()` converts the total seconds into minutes and seconds.
4. The timer decreases by 1 second after every second.
5. When the timer reaches zero, `"Fire in the hole!!"` is displayed.

## 💻 Code

```python
import time

def countdown(t):
    while t:
        mins, secs = divmod(t, 60)
        timer = '{:02d}:{:02d}'.format(mins, secs)
        print(timer, end='\r')
        time.sleep(1)
        t -= 1

    print("Fire in the hole!!")

t = input("Enter the time in seconds: ")

countdown(int(t))
```

## ▶️ How to Run

Make sure Python is installed on your computer.

Run the program:

```bash
python countdown.py
```

Then enter the time in seconds.

### Example

```text
Enter the time in seconds: 10

00:10
00:09
00:08
00:07
00:06
00:05
00:04
00:03
00:02
00:01

Fire in the hole!!
```

## 📚 Concepts Learned

This project helps beginners understand:

* Functions
* `while` loops
* User input
* Type conversion
* `divmod()`
* String formatting
* The `time` module
* Basic countdown logic

## 👨‍💻 Author

**C S Kartheek**

---

⭐ A beginner-friendly Python project for learning loops, functions, and time-based programming.
