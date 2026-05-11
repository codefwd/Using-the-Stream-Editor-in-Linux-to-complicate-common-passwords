# Using the Stream Editor in Linux to complicate common words or phrases as passwords.
**Never** use a word from a dictionary as a password, but if you do, there are ways to complicate it a little.
## Overview: We will look at the most common password wordlist used in Unix and Linux using the metasploit-framework. Then we will take ordinary words and *mung* them by replacing a number with a symbol or letter.
To start off, I will begin by opening a password list in Kali:<br/><br/>
<img width="795" height="176" alt="1" src="https://github.com/user-attachments/assets/ee8b7c6f-769f-4203-aed0-41e59e9d42b5" /><br/>
<img width="691" height="711" alt="2" src="https://github.com/user-attachments/assets/de56c117-ab54-4005-83ba-b3e87d3c85bb" /><br/>
As you can see that is way too many results. Going forward, you can use the **head** command instead of **cat** to get just the beginning of the results to make it a little more presentable.<br/><br/>
Before we attempt to do our munging, we need to get into root. I used *sudo su -* to get into root.<br/><br/>
<img width="279" height="93" alt="3" src="https://github.com/user-attachments/assets/4b113ced-3528-4720-9055-db9cc5953017" /><br/><br/>
So to start replacing all instances of the letter **a** with the **@** symbol, we will use the Stream Editor in Linux. It is the **sed** command. sed is equivalent to the Find and Replace in windows. The **sed** lets you search for occurrences of a word or pattern and then performs some action on it.<br/><br/>

<img width="1240" height="61" alt="4" src="https://github.com/user-attachments/assets/817634a2-d4a8-4845-943b-c4881e2e1df4" /><br/><br/>
To do the substitution - the **s** is used.
First, you give what you are searching for **(a)** and then what you want to replace it with **(@)**. Separate these with a fwd slash **(/)**.
To make it perform globally use the **g** flag. If you want only the first instance of **a** then leave off the **g**.<br/><br/>

Now show the new list and see the difference:<br/><br/>


<img width="617" height="83" alt="6" src="https://github.com/user-attachments/assets/e6a9698a-8171-4136-9074-023aca338996" /><br/><br/>

<img width="278" height="709" alt="5" src="https://github.com/user-attachments/assets/bea42200-6156-417b-a3bd-e025c371e744" /><br/>

In conclusion, By taking ordinary words and “munging” them—such as replacing letters with numbers or symbols—we can better understand how attackers modify common passwords to increase the chances of cracking them. This process highlights the importance of creating strong, complex passwords and reinforces the need for better password security practices in modern systems.
