# Torque Calculation for Robotic Arm

## Given Data:
1. **Arm Lengths:**
   - First arm: 15 cm = 0.15 m.
   - Second arm: 10 cm = 0.10 m.
   - Third arm: 4 cm = 0.04 m.

2. **Hanging Weight:** 1 kg.
3. **Gravitational Acceleration:** \( g = 9.81 m/s^2 \).

---

## Step 1: Calculate the Force (F)
The force acting on the arm due to the hanging weight is:

![image](https://github.com/user-attachments/assets/3c674e1c-5ea8-460e-a929-b4dc3ea9b634)

Substitute the values:

![image](https://github.com/user-attachments/assets/a3124e63-cf16-410b-a811-0e5d5426befb)


---

## Step 2: Calculate Torque for Each Joint
Torque at each joint depends on the force \( F \) and the effective length \( r \) from the pivot point.

### 1. Joint 1 (Base):
The base joint supports the torque caused by the hanging weight acting at each arm's center of mass. Torque at the first joint is:

![image](https://github.com/user-attachments/assets/97369e72-8fb6-413a-b2b3-5509c507ec45)

Substitute the lengths:

![image](https://github.com/user-attachments/assets/c11f5e81-a00c-4602-9d47-1f272a190e3c)


### 2. Joint 2 (Middle):
The middle joint supports the torque caused by the weight acting at the second and third arms:


![image](https://github.com/user-attachments/assets/55fa9b5b-5769-4ba0-8ae9-339a999af218)

Substitute the lengths:


![image](https://github.com/user-attachments/assets/8fb5d40e-705b-411d-9a8d-97bb3dbffd0b)


### 3. Joint 3 (End-Effector):
The end-effector joint supports the torque caused by the hanging weight at the third arm:


![image](https://github.com/user-attachments/assets/1b5ee472-b369-4bad-b4a6-534a2d1dee57)

Substitute the length:


![image](https://github.com/user-attachments/assets/2802f499-a4b5-4536-b058-380bacc749c4)

---

## Step 3: Select Suitable Motors
Based on the calculated torque values:
1. **For Joint 1 (Base):** Choose a motor with a torque rating higher than \( 2.8449 Nm\).
2. **For Joint 2 (Middle):** Choose a motor with a torque rating higher than \( 1.3734 Nm \).
3. **For Joint 3 (End-Effector):** Choose a motor with a torque rating higher than \( 0.3924 Nm\).

### Suggested Servo Motors:
- **For Joint 3:** Servo motor like MG996R (supports approximately ![image](https://github.com/user-attachments/assets/c07a7e68-38c9-442f-a982-e3f96d9e943c)
).
- **For Joint 1 and 2:** Use motors with higher torque ratings based on the requirements.

### Purchase Links:
- [MG996R Servo Motor on Amazon](https://www.amazon.com/s?k=MG996R)
- [High Torque Servo Motors](https://www.amazon.com/s?k=high+torque+servo+motor)
