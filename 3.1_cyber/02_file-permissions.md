# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

<img width="5712" height="4284" alt="IMG_5191" src="https://github.com/user-attachments/assets/0497dd5b-da76-43c8-ac9e-e32274c9d07d" />

(Add screenshot here)

### Questions

1.  Who owns the file?
2.  What are the default permissions?

### Reflection

Why is file ownership important in Linux systems?

------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

<img width="5712" height="4284" alt="IMG_5192" src="https://github.com/user-attachments/assets/80608101-9751-42f9-bb5d-e9b1c8a03dc2" />

(Add screenshot here)

### Questions

1.  Who can read the file now?
2.  Who cannot access it?


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

<img width="5712" height="4284" alt="IMG_5193" src="https://github.com/user-attachments/assets/8249995e-acc8-4cdf-88f6-47d4a7e10b16" />

(Add screenshot here)

### Questions

1.  Who can access the file now?
2.  Why might this configuration be dangerous?

