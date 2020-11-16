# [Coding an HTML5 Canvas Game with JS in 5 min 30 sec](https://www.youtube.com/watch?v=KoWqdEACyLI)

Tutorial followed from the video by Chris DeLeon of HomeTeam GameDev, published on December 30, 2015.

## Notes

- I was interested in following this tutorial despite its age because I wanted to familiarize myself with older coding conventions, with reading a new kind of code, and as a short break from completing my own projects (it does promise results in just over five minutes). I don't think I will rewrite this, at least not soon, since I am focusing on the HTML/CSS side of things. It is also only tangentially related to typical web dev, but that's what makes it a fun breather.

- The tutorial author *typed* twice as fast as I could follow, coding as he thought, and I was just barely keeping up with the broader concepts of what was done. I am so glad to hear his thoughts as he typed, because otherwise this is gibberish to me.

## Debugging

So, I made a horrible typo that was extremely awful. Instead of typing `cc.fillStyle='white';` when defining the color of the interactive elements of the game, I typed `cc.filStyle='white';`. EVERYTHING WAS BLACK. EVERYTHING WAS WORKING **BUT I COULDN'T SEE IT**.

Since there was no change of color, just an odd unused bit of code, all the game functions were working just fine, but I couldn't see the black-on-black because I missed typing an 'l', so I spent like fifteen minutes poring over the code and eventually just search and replacing all the variable names and other repeated text until I found the inevitable typo. And it wasn't even one of the super short variables. However, it felt **awesome** to have everything work *and* be able to see it.

## Things I Don't Understand (Yet)

- How does the AI speed work? I get that many of the variables were pixel values, but is the AI speed *also* a pixel value? It seems like it may be moving at 60 pixels per second (2 pixels * 30 frames per second), but I'm not completely sure.

- Where is the collision happening? Center of the ball, but where on each paddle?

- **Why** do JS developers use `e` as a variable? I see it all the time, but where does this come from? Is it culture-related like `foo` or language-related in some way?

## Enlightenment?

- I'm getting better at using `git`, and I am enjoying using it as a sub-blog level of informal writing. 

- I did follow much of the code, and I want to do more JS and even HTML/CSS tutorials like this one -- live explanation rather than chunks of code, chunks of documentation.
