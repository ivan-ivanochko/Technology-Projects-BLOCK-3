# Exploring the CIA Triad

## Objective

Understand the **Confidentiality, Integrity and Availability (CIA)** principles using practical tasks on a Raspberry Pi.

---

# Part 1 – Confidentiality

1. Create a confidential file.

    ```bash
    nano secrets.txt
    ```

1. Write some confidential information.

1. Save the file.

1. Now restrict access:
    ```bash
    chmod 600 secrets.txt
    ```
1. Check permissions:
    ```bash
    ls -l secrets.txt
    ```

**Questions**
- Who can read this file?
owner or root administrator 


- How does file permission protect confidentiality?
They stop other users and groups from reading or changing the file.

## Part 2 – Integrity

1. Create a hash of the file.
    ```bash
    sha256sum secrets.txt
    ```
    _What does "hash" do?

1. Save the output.

1. Modify the file.
    ```bash
    nano secrets.txt
    ```

1. Run the hash again.


** Questions**
- Did the hash change?
t turns data into a fixed-length "fingerprint". The same input always gives the same output, and any change gives a different one.
- Why do security systems use hashing?
  o detect tampering, verify file integrity and store passwords securely.


# Part 3 – Availability

1. Check system uptime:
    ```bash
    uptime
    ```

1. List running processes:
    ```bash
    top
    ```

**Questions**
- Why is system uptime important?
  Users and services depend on the system being available. High uptime means reliability.
- What happens if a system is unavailable?
  Services stop, which can mean lost productivity, lost revenue, damaged reputation and possibly data loss.

## Deliverables
Include:
SCREENSHOTS:

<img width="5712" height="4284" alt="IMG_5346" src="https://github.com/user-attachments/assets/93f0b580-30f0-460f-b8b8-683358640673" />
<img width="5712" height="4284" alt="IMG_5347" src="https://github.com/user-attachments/assets/b8ce50e9-3ffd-4925-a019-129addbb67d3" />
<img width="5712" height="4284" alt="IMG_5348" src="https://github.com/user-attachments/assets/a23e80d2-1788-40ec-b760-1a23579c3826" />
<img width="5712" height="4284" alt="IMG_5349" src="https://github.com/user-attachments/assets/b9e79ab2-9b2c-48e4-9d85-3229c8bfc8bb" />


















- Answers to questions
- Reflection
    >This activity demonstrated the three principles of the CIA triad through practical tasks on the Raspberry Pi.

Confidentiality. I created a file called secrets.txt and restricted access with chmod 600. This gives read and write permission only to the file owner and none to the group or other users. The ls -l output confirmed this (-rw-------). It showed me that confidentiality means only authorised people can access sensitive information, and that file permissions are a basic way of enforcing this.

Integrity. I generated a SHA-256 hash of the file, changed its contents and hashed it again. The hash changed completely, even though the edit was small. This showed me that hashing can detect unauthorised or accidental modification, so integrity means data stays accurate and unaltered. Systems use this to verify downloads, passwords and logs.

Availability. Using uptime and top, I checked how long the system had been running and which processes were using resources. This showed that a system must be running and accessible when users need it. Monitoring helps detect problems such as overloaded CPU or memory before they cause downtime.

Conclusion. The three principles work together. A system that is confidential but unavailable is useless, and data that is available but has been tampered with cannot be trusted. Good security needs a balance of all three.
