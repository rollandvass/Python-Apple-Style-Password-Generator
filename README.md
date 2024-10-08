# Secure Password Generator

This small application will generate you a secure 18 character password in the format of `XXXXXX-XXXXXX-XXXXXX`
Sound familiar? Yes, this is similar to how Apple generates passwords with their iCloud Keychain.

# How to use:

1. Download and extract: <br>

   - Click the green "Code" button to download the project as a ZIP file. <br>
   - After downloading, extract the ZIP file to your desired location.

2. Run the application: <br>
   - Navigate to the `dist` directory within the extracted files. <br>
   - Double-click `main.exe` to run the application. <br>
   - After generation, you can click the "Copy" button to copy your new password to the clipboard.

# CSV File Usage:

- If you use this app to generate your own passwords, the generated passwords will be saved in the `Python Passwords.csv` file. <br>
- You can easily import this CSV file into most browsers to manage your passwords.

# Security of the Passwords

These passwords are quite secure due to their length and randomness. The security of a password is determined by the total number of possible combinations an attacker would need to try (brute force) in order to guess the password. This is often referred to as the "entropy" of the password.

# Calculation of Entropy

1. Character Set Size: <br>
   Uppercase letters: 26 <br>
   Lowercase letters: 26 <br>
   Digits: 10 <br>
   Total: 62 possible characters

2. Password Length: <br>
   18 characters (excluding the dashes, which are not part of the entropy calculation).

3. Total Combinations: <br>
   The total number of combinations is $62^{18}$

Let's calculate that:
<br>
$62^{18} = 58,149,737,003,035,501,840,943,585,361,003,600$ <br>
This is approximately 58.15 quattuordecillion possible combinations.

# Time to Brute Force in 2024

The time it would take to brute-force such a password depends on several factors:

1. Attacker's Computational Power: <br>
   Let's assume a very powerful attacker with a setup capable of trying 100 billion guesses per second (which is a high-end estimate but feasible with state-of-the-art hardware and techniques).

2. Time to Crack: <br>
   The time to crack can be calculated by dividing the total number of combinations by the number of guesses per second. <br>
   $\text{Time to Crack} = \frac{58,149,737,003,035,501,840,943,585,361,003,600}{100,000,000,000\ \text{guesses/second}}$

This equals approximately: <br>
$\text{Time to Crack} = 581,497,370,030,355,018,409\ \text{seconds}$

Converting this into years: <br>
$\text{Years} = 581,497,370,030,355,018,409/31,536,000 \approx 18,435,299,434,000\ \text{years}$
​

# Conclusion

With these calculations, it would take an attacker approximately 18.4 trillion years to brute-force such a password with current technology, assuming 100 billion guesses per second. This time is vastly longer than the age of the universe, making the password effectively uncrackable by brute force with today's technology.

So, even though the password doesn't include special characters, its length and randomness make it extremely secure. Adding special characters could make it even stronger, but for most practical purposes, these generated passwords are more than sufficient in terms of security.
