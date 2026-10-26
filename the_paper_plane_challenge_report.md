# Technical Report: The Paper Plane Challenge

**Event:** IIT Bombay Techfest — Problem 2

## Part A — Design

### Wing Shape & Configuration
* **Configuration:** Broad wingspan with a blunt nose and flexible trailing edges.
* **Justification:** The broad wings maximize surface area. The loose trailing edges flutter (flap) under aerodynamic pressure during descent. This flapping acts as an airbrake, increasing drag to significantly slow the plane's vertical descent.

## Part B — Aerodynamics

### 1. Lift & Forces
* **Lift Generation:** Airflow is deflected downward by the wings' positive Angle of Attack during the glide phase.
* **Force Balance:** Initial manual **Thrust** overcomes **Drag** to achieve altitude. Once thrust drops to zero at the peak, gravity (**Weight**) pulls the plane down. This falling motion creates the necessary forward airflow over the wings to generate **Lift**, trading potential energy for time aloft.

### 2. Stability & Wing Loading
* **Wing Loading:** Minimizing wing loading ($W/S$) is the primary requirement for flight duration. By maximizing wing area with a standard 5g A4 sheet, the wing loading is extremely low, allowing it to float.
* **CG & Stability:** Folds are concentrated at the nose to keep the Center of Gravity (CG) ahead of the Center of Lift, preventing backflips. A slight dihedral (V-shape) was added for roll stability.

### 3. Minimum Sink Rate vs. Max Glide
A conventional "dart" optimizes for **Maximum Glide Distance** (low drag, high wing loading, fast forward speed). My flapping design optimizes for **Minimum Sink Rate**. It sacrifices horizontal distance, utilizing high induced drag and massive wing area to float downward as slowly as possible.

## Part C — Experiment

### 1 & 2. Flight Trials (Indoor, Wind-Free)
The objective was a high-angle, smooth launch to maximize initial altitude.

| Trial | Duration (s) | Observations | 
| :---: | :---: | :--- | 
| **1** | 4.06 | Good launch, steady flapping on descent. | 
| **2** | 4.60 | Excellent launch angle. Smooth glide path. | 
| **3** | 4.25 | Moderate altitude achieved, slight left bank. | 
| **4** | 3.95 | Stalled slightly at the peak climb before recovering. | 
| **5** | 4.40 | Consistent flapping action and slow sink rate. | 

**Mean Flight Duration: 4.25 seconds**

**Flight Videos:**
* [Test 1 Video (4.06s)](https://drive.google.com/file/d/1jamE_Ub25TG_moXkqFUD5oe_wmK6b0j7/view?usp=drive_link)
* [Test 2 Video (4.60s)](https://drive.google.com/file/d/1MR2xxZUpwtzKk4lhIEDt02Hv927xa3yR/view?usp=drive_link)

### 3. Suggested Modifications
1. **Winglets:** Fold the extreme wingtips upward by ~1cm. 
   * *Testing:* Compare mean flight times against the base model to see if reducing induced drag at the wingtips improves glide efficiency.
2. **Forward CG Shift:** Add one extra fold to the nose tip to increase front-weight.
   * *Testing:* Observe launch transition. This aims to prevent the peak-climb stall observed in Trial 4 by smoothing the leveling-out phase. All other launch variables (force, angle) would be held constant.