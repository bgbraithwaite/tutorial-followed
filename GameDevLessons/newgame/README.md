# [Coding an HTML5 Canvas Game with JS in 5 min 30 sec](https://www.youtube.com/watch?v=KoWqdEACyLI)

Tutorial followed from the video by Chris DeLeon of HomeTeam GameDev, published on December 30, 2015.

## Notes

I was interested in following this tutorial despite its age because I wanted to familiarize myself with reading and understanding pre-ES2015 conventions, and I needed a short break from my freeCodeCamp projects (it does promise results in just over five minutes). I may rewrite this, but not soon. I am focusing on HTML/CSS, and this is a fun breather only tangentially related to typical web dev.

## Debugging

The tutorial author moved at such a fast pace it was hard just to keep up with *typing*. He explained as he coded, and I only just grasped the broader concepts the first time through. After a few minutes, I had typed out the full project, but I had only a black box, with no paddles, text, or ball.

I got no errors in the developer consoles for Chromium or Firefox. CodePen's "Analyze JavaScript" button showed no errors. I was stumped.

I spent something like fifteen minutes poring over the code line by line, then I found an enhanced version in the YouTube comments to diff against line by line, *then* I searched and replaced all the variable names and other repeated text until I found the *inevitable* typo. And it wasn't even one of the super short variables! It felt *awesome* to have everything work *and* be able to see it.

Instead of typing `cc.fillStyle='white';` when defining the color of the interactive elements of the game, I had typed `cc.filStyle='white';`. *Everything* was black. The project was working properly the whole time, but I couldn't see it until I fixed a single missing 'l'.

## Things I Don't Understand (Yet)

- How does the AI speed work? I get that many of the variables were pixel values, but is the AI speed *also* a pixel value? It seems like it may be moving at 60 pixels per second (2 pixels * 30 frames per second), but I'm not completely sure.

- Where is the collision happening? Center of the ball, but where on each paddle?

- **Why** do JS developers use `e` as a variable? I see it all the time, but where does this come from? Is it culture-related like `foo` or language-related in some way?

## Enlightenment?

- The tutorial author coded and explained as he thought. There was a rhythm to it like when I play piano in flow state. Explaining aloud as I code seems like a particularly valuable communication skill to develop. I may even screen record myself to analyze my speech rythms and thought processes afterward, but that's a whole extra set of skills that I may not want to delve into while I'm already working on completing freeCodeCamp.

- This tutorial feels closest to what it's like inside the head of someone doing this for their work who is good at it, and I want more exposure to it by following more tutorials using the same format.

- I'm getting better at using `git`, and I am enjoying using it as a sub-blog level of informal writing. I practiced writing this README in `vim`, using simple editing shortcuts like `dd` and `p` to move lines around.

- `<canvas>` is less intimidating than I thought.

## Postscript

I took a break because I was having difficulty completing my next project (the technical documentation page). I have a clearer idea for what I want to do to finish it now, and I have a better sense of how to chunk my tasks. All told, I am glad I took this break! I got a lot more out of it than I thought I would going in.
