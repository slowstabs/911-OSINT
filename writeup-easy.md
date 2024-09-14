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

### Meta Daa-ta or Day-ta

> Christy told us about one image that he was supposed to get. What he had to recieve was not the image in itself but rather something in its metadata. The image was one that wasn't very uncommon but what was needed to him was the Universal Unique Identity of the image. The image is given below.
> He doesn't really need it anymore but you require points so help yourself :)

![image.jpg](https://github.com/user-attachments/assets/f1df2d5f-df11-46b3-9473-b1faf03f9cbc)


From the name of the challenge and the info given, its pretty clear that the solution deals with something realted to the metadata and Universal Unique Identity which if you search is the full form of UUID. If you have linux, you can run `exiftool` and get the metadata or if you're on Windows or something else, find an online tool for it. We find the UUID in the metadata which is what we require.

![image](https://github.com/user-attachments/assets/a3015b78-0409-49db-a66d-0b8a49c5df79)

Flag: `faf5bdd5-ba3d-11da-ad31-d33d75182f1b`

---

### Emergency

> Christy told us that Flight 77 crashing into the Pentagon caused all air traffic in the United States to shut down as per the instructions of the FAA. He recalls watching that on the TV on what was supposed to be one fine morning as one very traumatic one.
>
> He told us that it happened around the time he usually leaves for work, he couldn't remember the exact time the plane crashed into the Pentagon. Maybe you could help?

> Flag Format: hr:min:sec (In digits)

Another one that I hate ChatGPT for since it gave away the answer, but yeah shows how the future is.

The way I expected this to be solved was using a timeline which could be found on the britannica website

![image](https://github.com/user-attachments/assets/f2b8943a-5de1-4f47-9d2d-25ea893eb83e)

On searching for the keyword "Pentagon" we find what we're looking for.

![image](https://github.com/user-attachments/assets/3c3268e5-c6f5-4983-94b2-576caa9874a1)

#### Flag: 09:37:46

---



