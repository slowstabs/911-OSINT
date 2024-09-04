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

We could sit and decode it but for this I'll use chatgpt, and get the 5 numbers. The caption was hinting towards ascii and the numbers found also seem to come under the ascii aplhabets range so on running a decimal to ascii conversion, we get our first part - `ayman`

![image](https://github.com/user-attachments/assets/33cf964d-be30-4add-a219-4e839c8fc5ca)


The second one is pretty simple. It has the numbers `1 12` on the image and also a caption saying `Christy = 3 8 18 9 19 20 25`. Each of the letters are corresponding to the position in the alphabet (ie: a=1, b=2 and so on)

So `1 12` would be `al`









