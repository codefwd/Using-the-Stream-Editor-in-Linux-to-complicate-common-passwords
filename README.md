# Using the Stream Editor in Linux to complicate common words or phrases as passwords.
Momma always said, never use a word from a dictionary as a password, but if you do we can complicate it a little.
## Overview: We will look at the most common password wordlist used in Unix and Linux using the metasploit-framework. Then we will take ordinary words and *mung* them by replacing a number with a symbol or letter.
To start off, I will begin by opening a password list in Kali:<br/><br/>
<img width="795" height="176" alt="1" src="https://github.com/user-attachments/assets/ee8b7c6f-769f-4203-aed0-41e59e9d42b5" /><br/>
<img width="691" height="711" alt="2" src="https://github.com/user-attachments/assets/de56c117-ab54-4005-83ba-b3e87d3c85bb" /><br/>
As you can see that is way too many results. Going forward, you can use the **head** command instead of **cat** to get just the beginning of the results to make it a little more presentable.<br/><br/>
Before we attempt to do our munging, we need to get into root. I used *sudo su -* to get into root.<br/><br/>
<img width="279" height="93" alt="3" src="https://github.com/user-attachments/assets/4b113ced-3528-4720-9055-db9cc5953017" /><br/><br/>
So to start replacing all instances of the letter **a** with the **@** symbol we will use the Stream Editor in Linux. It is the **sed** command. It is equivalent to the Find and Replace in windows. The **sed** lets you search for occurrences of a word or word pattern and it then performs some action on it.
