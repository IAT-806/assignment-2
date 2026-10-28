# Assignment 2 — Body Game

Create a game with webcam and P5JS. Some kind of body interaction. It can be face, hands, body, etc, or something else.

**Due:** Monday, November 16th.

## What to make

It needs a **goal**. Something you are trying to do. A score, a timer, a way to win, a way to lose. It doesn't have to be all of these. But when someone plays it, it should be clear.

Make it fun and weird. Games where you look silly playing them are the best ones. **Bonus points** for weird. **Bonus points** if it makes the person playing it move in a way they normally wouldn't.

It's fine if it's simple.

Some ideas. Pick one, mix them, or invent your own:

- **Pop** the balls with your hands before they float away.
- **Dodge** things falling from the sky. Your silhouette is the thing that gets hit.
- **Catch** only the good things with your head. Avoid the bad ones.
- **Herd** a crowd of creatures into a corner with your arms.
- **Feed** a monster by bringing food to its mouth with your hand.
- **Hold a pose** to keep something alive.
- **Two players.** Two bodies, one camera.

## It must use

- [ ] **The webcam and an ml5.js model** — `bodySegmentation` (like in class), `bodyPose`, `handPose`, or `faceMesh`. Your body moves things in the sketch.
- [ ] **Object Oriented Programming** — the things in your game are objects, like our `Ball`. With a `constructor` and your own methods.
- [ ] **An array of objects** — many of them, made with a loop.
- [ ] **Adding and removing objects** — things appear, things disappear (`push()`, `splice()`). Popped, eaten, caught, spawned.
- [ ] **A score, a timer, or a goal** — a number or a state that changes when you play, shown on the screen with `text()`.
- [ ] **Game states** — at least a start and an end. Like `"start"`, `"playing"`, `"gameOver"`, with `if` / `else` in `draw()`.

### Bonus

- Levels. It gets harder the longer you play.
- Sound. You know how from Lab 03.
- Use two models at once. Your hands **and** your face.

## In class

I will ask some of you to play your game in front of the class, and then walk us through the code. Be ready to answer:

- Which ml5 model did you use? What does it give you back?
- How does your body touch the objects in your code? Show me the line.
- Where do objects get added? Where do they get removed?
- How do you win? How do you lose?
- What was hard? What broke? What did the camera get wrong?
- What surprised you?

If something doesn't work, that's fine. Bring it and we'll talk about it. That's how we learn.

## Some tips

- Plan ahead. Write what you want to do. In simple steps.
- Sketch it on paper. What's on the screen? What does the player do? What happens when they do it?
- Start from your Lab 06. You already have a class, an array, and a webcam working. Get your game working with the **mouse** first, then swap the mouse for your body.
- Look at the [ml5.js reference](https://docs.ml5js.org/#/reference/overview). Each model has a **Quick Start**. Run it on its own first, and look at what comes back in the console.
- Play your game. Play it again. Have a friend play it. Change what's boring.
- The camera is noisy. It loses your hand. It thinks a chair is a person. Make your game forgiving: bigger targets, a little slower, a few lives instead of one.
- The webcam is not mirrored, so moving your hand left moves it right on screen. That's confusing in a game. Look up the `flipped` option in the ml5 reference.
- Segmentation and pose models are heavy. If it's slow, use fewer objects or a smaller canvas.
- It is also a viable approach to start coding and see if something weird pops up.

## How to hand it in

Put it on your website as a new folder:

```
projects/iat-806/
├── lab-01/
├── ...
├── lab-06/
└── assignment-2/        ← your new one
    ├── index.html
    ├── sketch.js
    └── YourClass.js
```

Copy your `lab-06/` folder, rename it `assignment-2`, and make the game there. Edit the `index.html` in that folder: give it a title and write two or three sentences about the game. How do you play? How do you win? What part of your body do you use?

Add a link to it on `projects/iat-806/index.html`. Commit and sync. Check that it works at:

```
https://your-username.github.io/projects/iat-806/assignment-2/
```

The browser will ask for camera permission. GitHub Pages is `https`, so the camera works there.

In **Canvas**, submit:

1. The link to your live game in your website. It should include the link to your repo.

Need a reminder on adding a folder to your site? See [section 4 of the personal-website README](https://github.com/IAT-806/personal-website#4-add-a-submission).

## If something doesn't work

Open the browser console (right-click the page → **Inspect** → **Console**) and read the red text. The [If something doesn't work](https://github.com/IAT-806/Lab06#if-something-doesnt-work) section of Lab 06 covers the common ml5 and camera errors.

## On AI use

- You can ask questions from AI to explain things to you.
- Sometimes it's obvious if someone has used AI. If it's SUPER obvious, I'll reach out.
- Please don't just ask AI to make it for you. You have all the time in your life to do that later. Try to learn the basics. Write down code yourself. So you get some errors. So you can debug.
- Ask me, your friends, and the internet for help. You can ask AI to help you debug, but ask it to explain what is happening and why.
