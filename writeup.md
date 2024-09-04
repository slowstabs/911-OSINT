# 911/OSINT

## Easy

### K9

> Christy talked very highly of his friend Will Chesney and his dog and how brave they were. What was his loyal canine called?

Pretty simple challenge, all it takes is a google search and you have your answer. 

![image](https://github.com/user-attachments/assets/00c80d2d-4e25-4bce-83b7-c781ad160dbd)

Flag: `Cairo`

---


### Code Language

> Christy mentioned how Osama used to send messages in arabic which used to get translated into English but used to be sent in a ciphered format which used Caesar's cipher. Decoding this led to some discoveries related to his missions.
> One such message that he sent was "MNJNUVEV-UNF-SYRQ-QRAZNEX". What might this be in the decoded form?

In the challenge we have a string that doesn't make a lot of sense. The challenge mentions caesar's cipher which deals with letter shifting. So on using an online tool we can decode the answer.

![image](https://github.com/user-attachments/assets/94ebb6ea-5c2b-4ad5-91c5-e96d2a71e9e1)

But even after this, the answer didn't make sense, so we try shifting by little more or less and at 13 shifts we get a string that makes sense.

![image](https://github.com/user-attachments/assets/7eeefd45-7a2e-4d3e-bd5a-54bc862293b4)

Flag: `ZAWAHIRI-HAS-FLED-DENMARK`

---



