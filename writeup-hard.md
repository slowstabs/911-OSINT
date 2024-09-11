# 911/OSINT

## Hard

### Beeps and Boops

> Christy dealt with secret messages like the one in the challenge Code Language quite often and one which Christy fondly remembers, was when he deciphered an audio file to discover a major lead in the mission.
> He emphasised the satisfaction he got after understanding it and how it helped the progress, but didn't tell us what it was. Mind helping us out?

> Flag Format : xxxxx-xx-xxxxxxxx (Hyphens included)
> Attachments : horsecode.mp3

The challenge text doesn't really give us a lot of info on how to solve it so we can try analysing the `horsecode.mp3` file. On opening this file we hear *drumroll* beeps and boops! which sounds like morsecode. On running it through a morsecode translator we get the decoded message as `INSTAGRAM.COM/CHRISTYFBI`

![image](https://github.com/user-attachments/assets/3212827e-ed5f-4247-b456-55b584205d3e)

On going to that instagram profile we're greeted with 3 posts. Each post has some text and a caption, lets go through them one by one.

![image](https://github.com/user-attachments/assets/87847283-2234-4f5c-ba84-ea9e737bbcd2)

On the first one we're given a post with some random symbols on it and on the right we are given what seems to a paragraph in arabic. So quickly run a Arabic to English translate and we find the translated paragraph to be `The American Standard Code for Information Interchange is a character encoding standard for electronic communications. American Standard Code for Information Interchange symbols represent the text found in computers, communications equipment, and other devices.`

It hints towards American Standard Code for Information Interchange aka ASCII. But we still don't know what the symbols in the image are so we do a reverse image search through google lens and find out that the symbols are arabic numbers.

We could sit and decode it but for this I'll use chatgpt, and get the 5 numbers. The caption was hinting towards ascii and the numbers found also seem to come under the ascii aplhabets range so on running a decimal to ascii conversion:

We get our first part - **`ayman`**

![image](https://github.com/user-attachments/assets/33cf964d-be30-4add-a219-4e839c8fc5ca)


The second one is pretty simple. It has the numbers `1 12` on the image and also a caption saying `Christy = 3 8 18 9 19 20 25`. Each of the letters are corresponding to the position in the alphabet (ie: a=1, b=2 and so on)

**So `1 12` would be `al`**

Onto the last image. 

![image](https://github.com/user-attachments/assets/e44a908a-02c8-4416-8394-ec550444ef97)

In the caption it talks about Vigenere Cipher and how there's a key to cipher things.

In the image we see a key being equal pizza. We can find a tool online that converts vigenere cipher into normal text using a key. Since we have the text required with the key we can input the values and get the decoded message using an online tool like dcode.fr .

**The decoded message becomes `zawahiri`**

![image](https://github.com/user-attachments/assets/90fbb94a-3f6f-4027-bddd-645a0f722caf)

### So the total flag becomes **`ayman-al-zawahiri`**

---


### UGH THESE KIDS!

> Christy told us about a blunder that was noticed a few years after Bin Laden was killed when one Agent Hopper's teenage son Viki got access to some confidential info and made it public for fun.

> More about his son; he was a fan of DanTDM, a popular minecraft youtuber called Dan from back in the day. His birthday was on 21st July.

> His youtube channel name was inspired by the same youtuber and his birthday. Start by finding his Viki's YouTube channel.

This challenge is fairly simple after getting the first part, which is the name of Viki's channel. Using the info in the question you can see that the guy Viki followed was called DanTDM and Dan was the name of the youtuber. So if a guy is named Viki then his channel name would be? Yup VikiTDM. But that's not it we also got told that its consists of the birthday as well. So 21st July translates to 21/7 but you can't have symbols in youtube usernames so its just 217.

Note: Of course there could be multiple other combinations, but finding this was the challenge. It's not worth 150 points for nothing.

The final username comes to be vikitdm217.

On finding this channel on youtube we see that it has a video which was funny lolol, but on the community post has an email ID asking to mail to it.

![image](https://github.com/user-attachments/assets/fcbfe63e-bba0-493b-82fe-2c4288916eed)

We do as it says and after a few seconds you get a mail back with some information on it. 

![image](https://github.com/user-attachments/assets/cada2a52-90fb-42ac-b9f9-3eb65ee4f001)

In the image we see coordinates of some place and also a sentence hinting towards what3words (a website that names each pixel on the map with 3 random words)

So on inputting the coordinates into what3words, we get our flag :D

![image](https://github.com/user-attachments/assets/5debfb83-1ada-4e46-8bf6-23bb0b0f3135)

#### Flag: bleaching.twins.drooling

---

### Audio Spectrum

> Christy was a very keen learner and took interest in the creative ways Al-Qaeda sent secret messages. One such way was through spectrograms. Analysing them in a music software would show texts using waveforms.
> Here's one that Christy came across a while back, he asked me to try it myself but I'm a busy man so its on you!

We are given two files in the challenge, one is an audio and other is an archive file. The archive file seems to have a password so its ofc, we need to find that. In the questions spectrograms are mentioned so obviously, we observe the audio's spectrogram.

(I've used sonic visualiser, many of you guys used an online tool and it worked fine)

![image](https://github.com/user-attachments/assets/8f0f1ef8-7c08-4790-81a0-7d84cc75f71c)

It shows a pastebin link - pastebin.com/Umwrzvur. When we go here, we're greeted by a wall of text showing what seems to be an intercept of someone's call in urdu. So on translation we get : 

![image](https://github.com/user-attachments/assets/1118dd1c-e424-4d4e-b09b-e88d3b288096)

We see info about an AJ Traders in Lahore dealing with bathroom fittings, and tells us about a password which is a phone number of a shop with something related to "USA Tools" which wont show up on maps. We use google maps and find AJ traders.

![image](https://github.com/user-attachments/assets/d647fffa-fb27-4515-8cc8-f2bcc1d26b64)

So now we need to find USA tools which is not mentioned on maps, so we use street view to look around and find it.

![image](https://github.com/user-attachments/assets/e185f93a-0554-4868-89af-f34cbf08f819)

We see a phone number on a sign board of `Made in USA tools` being `0300 9456596`. We use this as the password for the archive we got in the beginning. The archive has an image and an instructions.txt. The image is a picture of a person and the instructions tell us that his full name without spaces is the flag. So we do a quick reverse image search and find the dude's wikipedia page, and voila we have the flag!

![image](https://github.com/user-attachments/assets/c40a1b54-cb8f-48d7-94c4-96e2919cf144)

####Flag: SyedAminulHaque


---

























