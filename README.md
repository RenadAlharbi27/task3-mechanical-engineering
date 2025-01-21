# Torque Calculation for Robotic Arm

## Given Data:
1. **Arm Lengths:**
   - First arm: 15 cm = 0.15 m.
   - Second arm: 10 cm = 0.10 m.
   - Third arm: 4 cm = 0.04 m.

2. **Hanging Weight:** 1 kg.
3. **Gravitational Acceleration:** \( g = 9.81 \, \text{m/s}^2 \).

---

## Step 1: Calculate the Force (F)
The force acting on the arm due to the hanging weight is:
\[
F = m \cdot g = 1 \cdot 9.81 = 9.81 \, \text{N}.
\]

---

## Step 2: Calculate Torque for Each Joint
Torque for each joint depends on the distance \( r \) from the pivot point and the load acting on it.

### 1. Joint 1 (Base):
- Supports the entire arm (hanging weight + weights of all arms).
- Torque at the first joint:
  \[
  \tau_1 = F \cdot r_{\text{Arm1}} + F \cdot r_{\text{Arm2}} + F \cdot r_{\text{Arm3}}.
  \]
  Using the lengths:
  \[
  \tau_1 = 9.81 \cdot 0.15 + 9.81 \cdot 0.10 + 9.81 \cdot 0.04 = 2.943 \, \text{Nm}.
  \]

### 2. Joint 2 (Middle):
- Supports the weight of the arm segments after it (third arm + hanging weight).
- Torque at the second joint:
  \[
  \tau_2 = F \cdot r_{\text{Arm2}} + F \cdot r_{\text{Arm3}}.
  \]
  Using the lengths:
  \[
  \tau_2 = 9.81 \cdot 0.10 + 9.81 \cdot 0.04 = 1.372 \, \text{Nm}.
  \]

### 3. Joint 3 (End-Effector):
- Supports only the hanging weight.
- Torque at the third joint:
  \[
  \tau_3 = F \cdot r_{\text{Arm3}}.
  \]
  Using the lengths:
  \[
  \tau_3 = 9.81 \cdot 0.04 = 0.392 \, \text{Nm}.
  \]

---

## Step 3: Select Suitable Motors
Based on the calculated torque values:
1. **For Joint 1 (Base):** Choose a motor with a torque rating higher than \( 2.943 \, \text{Nm} \).
2. **For Joint 2 (Middle):** Choose a motor with a torque rating higher than \( 1.372 \, \text{Nm} \).
3. **For Joint 3 (End-Effector):** Choose a motor with a torque rating higher than \( 0.392 \, \text{Nm} \).

### Suggested Servo Motors:
- **For Joint 3:** Servo motor like MG996R (supports approximately \( 10 \, \text{kg.cm} \) = \( 0.98 \, \text{Nm} \)).
- **For Joint 1 and 2:** Use motors with higher torque ratings based on the requirements.

### Purchase Links:
- [MG996R Servo Motor on Amazon](https://www.amazon.com/s?k=MG996R)
- [High Torque Servo Motors](https://www.amazon.com/s?k=high+torque+servo+motor)
