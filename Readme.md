# Breadth-First Search (BFS) – Pseudocode

This document outlines the pseudocode for the **Breadth-First Search (BFS)** algorithm, commonly used for graph traversal and shortest path discovery in unweighted graphs.

---

## Function Definition

```plaintext
Initialize system
Start camera feed

While application is running:
    Read video frame
    Convert to grayscale
    Detect faces and motion

    If face or motion detected:
        Update last_detection_time
        If appliance is OFF:
            Turn appliance ON
            Log activity
    Else:
        If last_detection_time exists:
            If time since detection > 10s:
                Show warning
            If time since detection > 15s:
                Turn OFF appliances
                Log activity
                Reset last_detection_time
    Update GUI
