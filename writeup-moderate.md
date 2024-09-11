# 9/11 OSINT

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

