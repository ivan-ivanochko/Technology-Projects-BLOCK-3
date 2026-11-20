# Password Security

## Task 1 --- Test a Weak Password

Run:

    echo "password123" | cracklib-check

<img width="5712" height="4284" alt="IMG_5194" src="https://github.com/user-attachments/assets/127fbec5-ffc5-4b55-a2e9-26549c3de26e" />

(Add screenshot here)

### Questions

1.  What does the tool say about the password?
2.  Why is this password weak?

### Reflection

Explain why weak passwords are dangerous.

------------------------------------------------------------------------

## Task 2 --- Test a Strong Password

Run:

    echo "Tr4!nBicyclePlanet" | cracklib-check

<img width="5712" height="4284" alt="IMG_5195" src="https://github.com/user-attachments/assets/3706e3b4-8e46-4925-bb13-0834bbdb817b" />

(Add screenshot here)

### Questions

1.  What result did the tool return?
2.  What characteristics make this password stronger?

### Reflection

Describe at least three characteristics of strong passwords.

------------------------------------------------------------------------

## Task 3 --- Password Analysis

Evaluate the following passwords:

-   123456
-   qwerty
-   P@ssword1
-   correcthorsebatterystaple

### Questions

1.  Which passwords are weak?
2.  Which password is strongest?
3.  Why?

### Reflection

Explain what you learned about password strength.

. Which passwords are weak?

123456: very weak. It’s consistently one of the most common passwords in breach lists, so it would be guessed almost instantly.
qwerty: very weak. It’s a keyboard pattern and also near the top of every common-password list.
P@ssword1: weak, despite looking “complex.” It’s just the word “password” with predictable substitutions (a → @) and a digit tacked on the end. Attackers’ cracking tools apply exactly these substitutions automatically.
correcthorsebatterystaple: not weak, as explained below.
