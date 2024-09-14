![image](https://github.com/user-attachments/assets/5a3162e2-c796-48e6-be89-5db9304c9448)# 9/11 OSINT

## Moderate

### Cassandra In Agony

> Christy told us that he and his wife had arguments and fights regarding his job, but knowing them I can assure you that Christy Annunziata and Cassandra R Annunziata are a wonderful couple.

> But its very true that Cassandra had very strong opinions about his job and had a strong disgust for the people Christy had to deal with. She is very vocal about it on social media, you have to check out her latest post on twitter, it's hilarious how easy it is to FLAG her alarms.

Since the question says twitter, that's where we go! On searching on twitter we find the twitter account of Cassandra R. Annunziata, with a post mentioning some document.

![image](https://github.com/user-attachments/assets/fb15c773-437e-48f9-b568-4fb1af77e0b2)

On looking at her website link , it leads to the CIA website which contained all the information gained from extraction of Osama's hard drive. Since in the post it mentioned document, we select docements at the bottom of the page and search for `suicide_bombing_attack` since it seemed like a suspicious looking string. 

![image](https://github.com/user-attachments/assets/e7530636-9eb0-4ea7-9546-72cdf3139a9b)

![image](https://github.com/user-attachments/assets/4d004332-1eba-45c6-98a2-3dd0312e6a09)

Since in the twitter post, Cassie said `his name really FLAGS my nerves`, if pretty obvious that the dude's name is the flag. Going through the PDF you'll find his name and there you have it.

![image](https://github.com/user-attachments/assets/c5465c7c-b80f-4f32-a3d8-67b9398d6a2b)

Tiny easter egg: The first letters of this challenge translate to CIA :)

#### Flag: Muaath al-Turki

---

### Simpsons Again!??

> In his interviews Christy mentioned that he found it very suspicious that Simpsons subtly predicted the attack. The controversy got so bad that the episode was banned for a few weeks. Christy hated the fact that it was so well rated on IMDb and ended up disliking all rating websites as a whole.
> 
> It bamboozled Christy how a TV show could predict an event that occured around 4 years before the actual event. Help Christy remember the exact date of this airing.
> 
> Oh! Oh! Also, Christy believes in fandoms :)

> Format: MM-DD-YYYY

I was surprised how so many of you got this so easily since I made this to be pretty hard. Turns out its just a ChatGPT prompt away. Well nothing wrong in that, its not open source if I say you we're not allowed to use AI. 

Anyways the way I thought you would take is search for the episode then go to the simpsons.fandom.com page and find the date but its ok, freebie I guess lol

![image](https://github.com/user-attachments/assets/c111a537-d3e8-4d10-86f4-f1cbd8bc226c)

#### Flag: 09-21-1997

---

### Myth Busters

> Christy's wife was one very curious one and searches about Christy's current and past works a lot.
>
> Christy had told his wife about one dude on reddit who explained how much preparation was put into the execution of Bin Laden.
>
> Christy remembers that it started from reading a post on why did the SEALS kill Osama Bin Laden on the spot on a sub reddit. And the guy he's refering to happened to be the top reply of the top post of all time in that subreddit.

> Wish he remembered the dude's name tho man, shucks :(


Since we have the path that Christy took to find the guy, we can follow his footsteps! Starting from the post with `why did the SEALS kill Osama Bin Laden on the spot`. You can find this post by searching that using google dorking or just mentioning reddit in the search query.

![image](https://github.com/user-attachments/assets/cc5fbfb5-0825-46bb-aec4-0c208941180c)

The post is in a subreddit called r/WarCollege. By just going to the main page of the subreddit, sorting it by Top of All Time, we get the top post. The flag is hinted to be the username of the person who had the top reply on that post. And that happpened to be `blackhorse15A`, there you have it!

![image](https://github.com/user-attachments/assets/c8780ba5-a1f0-42ad-a782-f72e85fe9547)

#### Flag: blackhorse15A

---

### FBI.jpg

> In an interview after the tragedy, Christy from the Federal Bureau of Investigation mentioned putting out images regarding 9/11 onto the FBI vault on Sept 14th 2011, which confirmed debris from an American Airlines flight.
>
> One of the images happened to have a serial number in it, which Christy remembers seeing but doesn't remember, maybe you could help?

> Hint: M_________ and they're all digits?? UGH I HATE THE DUDE WHO MADE THIS CHALLENGE

This was one I saw a lot of you struggle with and I don't blame you, it was a little confusing.

From the question we get that we need to find the images regarding 9/11 that were put into the FBI vault. On search we find out that the FBI vault is used as an archive to store old data. On a quick google dork search on the vault website we find a link which looks like something we need.

![image](https://github.com/user-attachments/assets/1f9d1657-0efe-4ce9-95a2-55138bef79eb)

Going through the images on that website, we find the image we are looking for with a serial number. The part you people struggled with was figuring out what the number was. I expected you guys to just try all the permutations and find the answer which some of you did do, so well done. 

It's just typing what you can see. The hint told us that after the M its just digits and also a particular number of underscores denoting the amount of digits (nine)

#### Flag: M005537944

---

### 1998

> Christy mentioned in his interviews that the FBI had performed investigations on Osama or rather Usama as he was called then, much before the event of 2001.
>
> In the first out of a three part record consisted of the FBI in early 1998 investigating the actions of Bin Laden along with his biodata, spottings and also his then assumed accomplices which were put into the FBI Vault.
>
> Christy also mentioned that the Control No. of the case was considered very confidential, but in 2024 its not. And you happen to be pretty curious right?

Even this one requires us to search the FBI Vault so another quick google dorking seach using the info we have like "first out of a three part document"

![image](https://github.com/user-attachments/assets/096db60a-98bb-4fd5-a686-47ca82cef369)

Going through the document a little bit we find what we are looking for

![image](https://github.com/user-attachments/assets/136a6498-fe8d-4772-9ebc-e0db6b9b751a)

#### Flag: A-268/5-1998

---

### Pakistani Journalist

> Christy mentioned a pakistani journalist who interviewed Bin Laden in 1997. In the interview, Bin Laden mentioned his plans towards the United States, his ideas of Jihad and Al-Qaeda's mission.
>
> Christy said "There's a very historic image of Bin Laden with the interviewer with a rifle in the background on his wikipedia page". This gun was one that was retrieved from the Spetsnaz forces, after Mujahidin's victory over the Soviets. The gun's model was ____ ?

Firstly, the number of underscores is put there to trick you because the obvious answer I expected you guys to give was AK47 and it was very much the case.

How you solve this is using the info in "There's a very historic image of Bin Laden with the interviewer with a rifle in the background on his wikipedia page". So we need to go to Osama's wikipedia page. On a slueth of his page, we can find exactly what we're looking for in a picture where Pakistani journalist Hamid Mir is interviewing Bin Laden with a gun in the back and the model of the gun is also mentioned.

![image](https://github.com/user-attachments/assets/4d4834f1-c15e-402a-b54d-6aeee1d4a0d1)


#### Flag: AKS-74U

---


