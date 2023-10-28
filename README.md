# How-Cool-Is-ChatGPT-and-the-importance-of-Prompt-Engineering

Hello, today I was studying the japanese alphabet and decided to test if Chat GPT would be able to create a simple, yet functional way for me to practice what I had been studying.
There are multiple online games to practice the japanese alphabet but this time I asked chat GPT to code me a website (html + css + js) that would show a japanese character and the
user would need to input the correct romanization of the word.

Anyone who has tried to ask Chat GPT for complex stuff has already dealt with a lot of disappointment and frustration with its wrong and absurd answers. However, with the use of
the prompt engineering technique, it is possible to help Chat GPT to give us a more desired answer. The general idea is to give the most explicit details and information about the 
task you want it to perform. In addition to that, it is also desired to give some simple examples, so that Chat GPT understands better what is the task it is being asked.

I was able to get a nice and functional code by writing commands to Chat GPT only twice (well actually thrice but the last time was due to its sassiness). Below were my commands to
Chat GPT:

1- First Command:
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
"I want you to write me an html , css and java script file (of course if needed)

I want you to create an website that will show on the screen one of the characters from japanese hiragana or katakana. then the user will need to type the romanized writing for that japanese character.
For example: if on screen there is the character て then the user should type te

If the user guesses the character correctly, I want the screen to flash green, then show a different japanese character. I want this to go on forever. I want it to be a kind of game to practice the
user's japanese.

If the user types the incorrect answer, then I want the screen to flash red but remain with the same character on screen until the user types the correct character."
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

The code returned by Chat GPT looked alright but it was possible to notice two big flaws: It did not add the code to associate each japanese character with their corresponding romanization form,
and secondly it did not implement any code to check whether what was typed was correct or not therefore, no matter what the user inputted, the game would assume it was wrong.
And so I wrote in the command prompt a second time in order to see if Chat GPT would fix these major issues.

2- Second Command:
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
"I see that you made this variable

const characters = ["あ", "い", "う", "え", "お", "か", "き", "く", "け", "こ", "さ", "し", "す", "せ", "そ", "た", "ち", "つ", "て", "と"];

However, here is not included EVERY hiragana character and there are also 0 katakana characters. In addition to this mistake, you did not add the code that checks whether the user inputted the right
romanization of the character.
My suggestion is that you create an object where each key is a different japanese character and their respective values are their romanization. 
This way, in the javascript code, you can get a random key from this object and store their respective value in another variable. and then once the user inputs their answer, the program should check
if what was type corresponds to the value respesctive to the current key."
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

This time, chat GPT returned the final code that I have included in this repository. There was only one problem which was the fact Chat GPT had not included every single japanese hiragana and katakana
character. So I wrote one more time on the command prompt asking for it to give me the correct object with all the characters and their corresponding romanization.

3- Third Command:
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
"this works marvelous!

may I ask you to provide me with an object that contains every single katana and hiragana character as key and their values corresponding to their romanization form please"
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

Well, After this, it returned the correct java script object and with it, the website/game was done. This was a very simple task, which I could have very well implemented by myself.
However, the beauty of Chat GPT lies in the fact I managed to get this game working in less than 5 minutes, whereas if I were to code myself it would have taken around 1 hour.
So with the help of Prompt Engineering, I was able to obtain a nice and functional game to practice with my studies without much work or sweat! Thanks Chat GPT! 
