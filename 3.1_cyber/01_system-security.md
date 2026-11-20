# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

<img width="4284" height="5712" alt="tempImagearuq8d" src="https://github.com/user-attachments/assets/96338404-7383-430f-a18a-32ba8598708a" />




(Add screenshot here)

### Questions

1.  How many users exist on the system?
2.  Which accounts appear to be system accounts?
3.  Why do operating systems create system accounts?

### Reflection

Explain why understanding system users is important for cybersecurity.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

<img width="4284" height="5712" alt="tempImagepyKxXF" src="https://github.com/user-attachments/assets/1e33dc55-845d-448a-9578-2e8aeb1894ab" />

<img width="4284" height="5712" alt="tempImageLQ87od" src="https://github.com/user-attachments/assets/ae15fe11-9e2d-4a4b-84b8-88fa41c1e942" />




(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
2.  Why can processes running as root be dangerous?
3.  What could happen if a malicious program ran with root privileges?

### Reflection

What did you learn about system processes and security?

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

<img width="5712" height="4284" alt="IMG_5190" src="https://github.com/user-attachments/assets/49a7e4bc-b67e-4de3-8eb6-eb05a72e0463" />

(Add screenshot here)

### Questions

1.  Which ports are open?
2.  Which services appear to be listening?
3.  Why might open ports represent a security risk?

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
