# Breadth-First Search (BFS) – Pseudocode

This document outlines the pseudocode for the **Breadth-First Search (BFS)** algorithm, commonly used for graph traversal and shortest path discovery in unweighted graphs.

---

## Function Definition

```plaintext
1. Start Video Capture
2. Loop:
Capture and flip the current video frame.
Convert frame to grayscale.
Apply:
Face detection using Haar Cascade.
Motion detection using background subtraction.
If face or motion is detected:
Update last_detection_time.
Turn ON all appliances not already ON.
Log the ON event.
Else:
If last_detection_time exists:
Calculate elapsed time.
If elapsed > 10s, show warning message.
If elapsed > 15s:
Turn OFF appliances.
Log the OFF event.
Reset detection timer.
If no detection timer exists, display “Detecting...” status.
Update GUI with new camera frame and appliance icons.
Wait 10 ms and repeat.
3. Admin Interaction (via GUI)
Login, view logs, export data, and access appliance usage graphs.
