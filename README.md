# 🔐 Password Gate Lock System

An Arduino-based password authentication system designed to provide secure access control for gates, doors, and personal lockers. The system accepts a password through a keypad, displays the system status on a 16×2 LCD, and operates a servo motor when the correct password is entered.

---



## 📌 Project Overview

The **Password Gate Lock System** is an embedded security project that provides password-based access control.

The user enters a password using a keypad. The Arduino compares the entered password with the password stored in its memory. If the password is correct, the servo motor operates the locking mechanism and grants access. If the password is incorrect, access is denied and an alert can be provided through a buzzer.

---

## 🎯 Objectives

- To develop a secure password-based access-control system.
- To protect gates, doors, lockers, and other restricted areas.
- To provide a simple and user-friendly authentication mechanism.
- To control a physical locking mechanism using a servo motor.
- To display password and access status using a 16×2 LCD.
- To demonstrate the practical application of Arduino and embedded systems.

---

## 🧩 Components Required

- Arduino Uno
- Matrix Keypad
- 16×2 LCD Display
- Servo Motor
- Buzzer
- Connecting Wires
- Power Supply
- Gate/Lock Prototype

---

## 🏗️ System Architecture

```text
              +------------------+
              |   Matrix Keypad  |
              +--------+---------+
                       |
                       v
              +------------------+
              |    Arduino Uno   |
              |                  |
              | Password Compare |
              +----+--------+----+
                   |        |
             +-----+        +------+
             |                     |
             v                     v
     +---------------+     +---------------+
     |    16×2 LCD   |     |    Buzzer     |
     |    Display    |     |     Alert     |
     +---------------+     +---------------+
                   |
                   v
             +----------------+
             |  Servo Motor   |
             | Lock Mechanism |
             +----------------+
