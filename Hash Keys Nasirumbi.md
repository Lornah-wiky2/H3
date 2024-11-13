## € Schneier 2015: Applied Cryptography: Chapter 2 - Protocol Building Blocks: subchapters "2.3 One-way Fuctions" and "2.4 One-Way Hash Functions"
#### key concepts in cryptography
One-way functions are operations that are easy to perform in one direction but extremely difficult to reverse, like breaking a plate into pieces. 
           Trapdoor one-way functions, These have a secret key that allows for easy reversal. 
Hash functions are tools that convert variable-length input into fixed-length output.     
These functions are easy to compute but hard to reverse, making them valuable for verifying data integrity without revealing the original information. 
Message authentication codes (MACs). These are hash functions that incorporate a secret key for added security. 
Overall, these cryptographic tools serve as fundamental building blocks for many modern security protocols and applications
### Reference:
https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003 


## Karvinen 2022: Cracking Passwords with Hashcat
#### How to crack password hashes using a tool called Hashcat. 
Password hashes are scrambled versions of passwords that can't be directly reversed.
The article demonstrates how to install Hashcat, obtain a dictionary of common passwords, identify the type of hash, and then use Hashcat to try every word until it finds a match.
 It uses a simple example of cracking the hash "6b1628b016dff46e6fa35684be6acc96", which is the password "summer". 
This process involves running commands in a Linux terminal, and emphasis is put on the importance of legal and ethical considerations when using such tools. 
computer's graphics card can significantly speed up the cracking process.
### Reference
https://terokarvinen.com/2022/cracking-passwords-with-hashcat/ 

## Voluntary bonus article (but recommended if you're not familiar with Linux command line): Karvinen 2020: Command Line Basics Revisited
This document provides a beginner-friendly introduction to essential Linux command line operations. It covers basic navigation commands like pwd (print working directory), ls (list files), and cd (change directory), as well as file manipulation commands such as mkdir (make directory), mv (move/rename), cp (copy), and rm (remove)
The guide also talks about remote access using SSH, viewing help documentation, and package management for installing software
Throughout the document, practical examples are given to illustrate each command's usage, making it easier for newcomers to understand and apply these fundamental Linux skills in their day-to-day interactions with the command line interface
### Reference 
https://terokarvinen.com/2020/command-line-basics-revisited/  

## A). Billion dollar busywork. Command 'echo -n "hello"|sha256sum' prints a hash. Try adding something to the string, e.g. 'echo -n 'hello asdf'|sha256sum'. What do you have to add to get a hash that starts with a zero?
![H3 hash that starts with zero](https://github.com/user-attachments/assets/02820a62-ddd1-43ef-913f-5f467617c3cb)
i tried multiple times and when i added 78 to the command that is when i got a zero at the beginning of the hash.

## B). Compare hash. Create a small text file. Take it's hash (e.g. 'sha256sum tero.txt'). Change one letter. Take the hash again. Compare hashes. What do you notice?
![H3 compare hashes](https://github.com/user-attachments/assets/98ea5c98-b30e-49df-b64a-59c7d1907f76)
i created a text then i hashed it. After i changed one letter in the same text. this changed the whole hash.

## C). Hashcat. Install hashcat and test that it works.
I found it challenging working with this . i kept getting the error not enough memory for this attack. Tried to boot terminal alone still getting same error.
here is the command i used.![boot terminal only](https://github.com/user-attachments/assets/997d7cfb-54ab-4343-affc-36658e11e3a2)


![error after boot terminal (not enough memory)](https://github.com/user-attachments/assets/a0c5f83d-6388-4d63-824e-f9cf80044621)

however it shows the hash works but there is just not enough space to run it.
![h3  hashcat works](https://github.com/user-attachments/assets/ca53a3ef-f43d-448e-831f-62a35a571879)


## D). Dictionary attack. Crack this hash: 21232f297a57a5a743894a0e4a801fc3
Getting error of not enough memory to perform this attack. 
![dictionary attack error](https://github.com/user-attachments/assets/fb50d424-b302-4d58-9bb1-305742a75e82)

## E). How can you make a password that's protected against a dictionary attack?
 Password managers are generally considered safe and are recommended by cybersecurity experts as an effective way to manage and secure passwords. 
 They work by encrypting and storing your passwords in a secure vault, which can only be accessed with a master password. 
 Most password managers use strong encryption methods like AES-256 and employ zero-knowledge architecture, meaning even the provider cannot access your data. 
 To maximize security, it's crucial to use a strong, unique master password and enable multi-factor authentication. 
 While no system is 100% secure, the benefits of using a password manager far outweigh the risks of not using one, as they allow you to create and use strong, unique passwords for each account without having to remember them all.
