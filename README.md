## Narrow-Phase Collision Detection (GJK & SAT)

This project explores **narrow-phase collision detection** by implementing two fundamental algorithms commonly used in computer graphics and game engines.

### Algorithms

**SAT / OBB (2D)**  
Collision detection and penetration resolution for oriented 2D shapes using the **Separating Axis Theorem**.

**GJK (3D)**  
Robust collision detection between arbitrary **convex 3D shapes** using the **Gilbert–Johnson–Keerthi algorithm**.

### Design Notes

For **2D**, collision detection is implemented using SAT with oriented bounding boxes and convex polygons.

While SAT can be extended to **3D**, it does not scale well in practice.  
As a result, **GJK is typically preferred for 3D convex collision detection**.

### Implementation & Visualization

Both algorithms are implemented **from scratch in Unity**, with a focus on learning and understanding the underlying mechanics.

- For **SAT**, the **Minimum Translation Vector (MTV)** is computed and visualized to show penetration depth and resolution direction.
- For **GJK**, only **collision states and world-space vertices of the involved convex shapes** are visualized.  
  *(Simplex visualization and MTV extraction via EPA are not implemented.)*
