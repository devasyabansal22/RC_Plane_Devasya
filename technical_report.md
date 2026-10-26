# Technical Report: Airfoil Selection for RC Aircraft
**Event:** IIT Bombay Techfest — Problem 1

## 1. Candidate Airfoils
The two aircraft have very different goals. Aircraft A needs to carry a heavy weight and fly stably. Aircraft B needs to do quick turns, loops, and fly upside down.

*   **Aircraft A (Max Payload):** We need an airfoil that generates a lot of lift at low speeds. 
    *   *Shortlist:* Selig S1223, Eppler 423, Clark Y.
*   **Aircraft B (Maneuverability):** We need an airfoil that behaves the same way upright or inverted, with predictable stalls.
    *   *Shortlist:* NACA 0012, NACA 0015, Eppler 168.

## 2. Final Selection & Justification
**Aircraft A: Selig S1223**
I selected the Selig S1223 for the heavy-lift plane. It has a highly curved "undercambered" shape (the bottom is scooped out). This design forces a lot of air downward, creating massive lift even at low speeds. It is a standard choice for heavy-lift RC competitions because it can carry heavy payloads without needing complex flaps.

**Aircraft B: NACA 0015**
I selected the NACA 0015 for the aerobatic plane. It is perfectly symmetrical (0% camber), meaning the top and bottom look exactly the same. This is crucial for aerobatics because the plane will fly upside down just as easily as right-side up. I chose the 0015 over the thinner 0012 because the extra thickness makes the plane stall more gently, which helps maintain control during crazy maneuvers.

*[Insert Diagram 1: Cross-section image of the Selig S1223 and NACA 0015 here]*

## 3. Comparison Table

| Feature | Aircraft A (Selig S1223) | Aircraft B (NACA 0015) |
| :--- | :--- | :--- |
| **Lift Coefficient** | Very High | Moderate |
| **Drag** | High | Low (when flying straight) |
| **Shape (Camber)** | Highly Curved (Undercambered) | Symmetrical (0% curve) |
| **Thickness** | 12.1% | 15.0% |
| **Stall Behavior** | Sharp and sudden | Gentle and predictable |
| **Inverted Flight** | Very poor | Excellent |

## 4. How Geometry Affects Performance
The physical shape of the wing directly controls how the plane flies:
*   **Camber (Curve):** More curve (like the S1223) means more lift, but it creates a lot of drag. Zero curve (like the NACA 0015) means less drag, but the plane has to tilt its nose up to generate lift.
*   **Thickness:** Thicker wings (like the NACA 0015) allow the air to flow around the edge smoothly even at high angles, which prevents sudden stalls.

## 5. Can One Airfoil Do Both?
You *could* use a semi-symmetrical airfoil like the **Clark Y** for both planes, but it would be a bad compromise. It wouldn't generate enough lift to win the heavy payload mission, and it would be much harder to fly upside down during the aerobatics mission. For a competition, it is much better to have specialized wings.

## 6. Airfoil (2D) vs. Whole Aircraft (3D)
It is important to remember that the airfoil is just a 2D cross-section. The actual performance depends on the whole 3D plane:
*   **Wing Loading:** How much weight is spread over the wing area. A great airfoil won't save a plane that is too heavy for its wing size.
*   **Control Surfaces:** The airfoil doesn't make the plane roll; large ailerons and strong servos do.
*   **Thrust:** A heavy-lift wing creates a lot of drag, so the plane needs a powerful motor to keep moving forward.

## 7. Bonus: XFLR5 Computational Analysis
To back up these choices, I ran the airfoils in XFLR5 at a Reynolds Number of 300,000, which is standard for RC planes of this size.

*   **Assumptions:** The flow is at low speed (Mach ~0) and standard air density. 
*   **Results:** The Cl vs Alpha graph showed the Selig S1223 generating huge lift at 0 degrees, while the NACA 0015 generated zero lift at 0 degrees, proving its symmetry. The Drag Polar graph showed the S1223 has much higher drag across the board compared to the NACA 0015.

*[Insert Diagram 2: Screenshot of XFLR5 Cl vs Alpha graph comparing both airfoils]*

## References
1. AirfoilTools.com (For airfoil coordinates and basic polar data).
2. XFLR5 v6.5 (Used for aerodynamic simulation and graphs).
3. Anderson, J. D. *Fundamentals of Aerodynamics*.