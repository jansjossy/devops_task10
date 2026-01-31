
# devops_task10
# DevOps Internship - Task 10: Volumes & Networking
**User:** Janzj

## 1. Docker Volumes (Data Persistence)
- **Concept:** Volumes decouple storage from the container lifecycle.
- **Test:**
    1. Created volume `my_safe_storage`.
    2. Wrote "This data survives" to `/data/secret.txt` in Container A.
    3. Deleted Container A.
    4. Mounted the same volume to Container B.
- **Result:** Container B successfully read the file, proving data persistence.

## 2. Docker Networking
- **Concept:** User-defined bridges allow automatic DNS resolution between containers.
- **Test:**
    1. Created network `my_custom_net`.
    2. Launched `target-container` on this network.
    3. Pinging `target-container` from a neighbor container worked immediately.
- **Diagram:**
    [Container A] <---(my_custom_net)---> [Container B]

## 3. Evidence
<img width="960" height="1020" alt="Screenshot 2026-01-31 100554" src="https://github.com/user-attachments/assets/532eac43-7b2d-4de9-8c8e-f612418ab49d" />
<img width="960" height="1020" alt="Screenshot 2026-01-31 100235" src="https://github.com/user-attachments/assets/c760b2a5-bbf5-46d5-8141-0a57b5e5d8e9" />
<img width="931" height="1020" alt="Screenshot 2026-01-31 101722" src="https://github.com/user-attachments/assets/1dc529a3-c103-4267-bc59-bf5a1006255c" />
<img width="931" height="1020" alt="Screenshot 2026-01-31 101716" src="https://github.com/user-attachments/assets/a325c08d-0757-4463-b62b-2f84790ae0e9" />

