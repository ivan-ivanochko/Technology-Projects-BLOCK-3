# Password Security

## Task 1 --- Test a Weak Password

Run:

    echo "password123" | cracklib-check

<img width="5712" height="4284" alt="IMG_5194" src="https://github.com/user-attachments/assets/127fbec5-ffc5-4b55-a2e9-26549c3de26e" />

(Add screenshot here)

### Questions

1.  What does the tool say about the password? Typically: password123: it is based on a dictionary word (some versions say “it is too simplistic/systematic”). The tool rejects it.
2.  Why is this password weak? It is built from the dictionary word “password”, the most common password there is, with the predictable suffix “123” added. Attackers try exactly these combinations first.

### Reflection

Weak passwords are dangerous because they are guessed in seconds by brute-force and dictionary attacks. Once one is cracked, attackers can take over the account, steal data, and try the same password on other sites (credential stuffing), especially when people reuse it.
------------------------------------------------------------------------

## Task 2 --- Test a Strong Password

Run:

    echo "Tr4!nBicyclePlanet" | cracklib-check

<img width="5712" height="4284" alt="IMG_5195" src="https://github.com/user-attachments/assets/3706e3b4-8e46-4925-bb13-0834bbdb817b" />

(Add screenshot here)

### Questions

1.  What result did the tool return? Typically: Tr4!nBicyclePlanet: OK. The tool accepts it.
2.  What characteristics make this password stronger? It is long (18 characters), mixes uppercase, lowercase, digits and a symbol, and combines unrelated words (“Train”, “Bicycle”, “Planet”) instead of one dictionary word. It does not match a common pattern.

### Reflection

Three characteristics of strong passwords:

Length. Longer is harder to crack; 12+ characters is a good minimum.
Unpredictability. No dictionary words, names, dates, or keyboard patterns.
Uniqueness. A different password for every account, ideally kept in a password manager.
------------------------------------------------------------------------

## Task 3 --- Password Analysis

Evaluate the following passwords:

-   123456
-   qwerty
-   P@ssword1
-   correcthorsebatterystaple

### Questions

1.  Which passwords are weak? 123456: very weak. It is one of the most common passwords in breach lists and is guessed almost instantly.
qwerty: very weak. It is a keyboard pattern near the top of every common-password list.
P@ssword1: weak, despite looking “complex”. It is just “password” with predictable substitutions (a → @) and a digit added. Cracking tools apply these substitutions automatically.
correcthorsebatterystaple: not weak.
2.  Which password is strongest? correcthorsebatterystaple.
3.  Why? It is very long (25 characters) and made of four unrelated words, which gives high entropy (roughly 44-51 bits if the words are truly random). It is not a single dictionary entry or a common pattern, and it is easy to remember and type. Caveat: this exact phrase is famous (from the XKCD comic), so attackers have it in their wordlists. The method is strong, but the phrase itself should never be used.

### Reflection

Length and unpredictability matter more than looking complex. P@ssword1 has symbols but is easy to crack, while a long random passphrase is both strong and memorable. Attackers guess the most likely passwords first, so a password’s strength is really how unlikely it is to be guessed. Even a strong password needs to be unique per site and protected with multi-factor authentication.
. Which passwords are weak?

123456: very weak. It’s consistently one of the most common passwords in breach lists, so it would be guessed almost instantly.
qwerty: very weak. It’s a keyboard pattern and also near the top of every common-password list.
P@ssword1: weak, despite looking “complex.” It’s just the word “password” with predictable substitutions (a → @) and a digit tacked on the end. Attackers’ cracking tools apply exactly these substitutions automatically.
correcthorsebatterystaple: not weak, as explained below.
