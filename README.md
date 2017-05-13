Peg Board: A beads toy in your browser
======================================

This is a personal weekend project finished in 3 hours.

This is where it starts. My wife bought a toy named "Bitsy Beads".
It is about putting tiny colorful rings on a peg board to form pictures,
something like this picture:

![beads on board](https://scontent.cdninstagram.com/t51.2885-15/s640x640/sh0.08/e35/12912785_624770734343891_452862785_n.jpg?ig_cache_key=MTIzMjg0NTI3MzM4MzAyMjU3MQ%3D%3D.2).

Then she and the kids spend some happy time on it during the weekend.
That gave me the idea of "what if I code this game on my computer?".
So I set off.

First of all, I was never a game developer, so I don't have the skillset to develop a polished game.
I did work on some web projects which (inevitably) including jQuery,
but I am not a front end developer either.
So, naturally I tend to use old school HTML table cells to represent the peg board,
and use jQuery to catch the onClick event and then change cell background color.
That would work, but I can already foresee the workload in jQuery will probably be tedious:
defining cells with IDs, bind listeners on them, maintain and update cell status.
(More on this later.)

So I consider AngularJS, a Javascript framework I was briefly introduced to at 5+ years ago.
With the help of this [online tutorial](https://www.w3schools.com/angular/angular_model.asp)
I've been able to finish this proof-of-concept in 3 hours.
I'm happy with my new toy, as happy as my wife and kids are with theirs.

Thoughts:

1. I just skimmed over the first half of the tutorial to complete this PoC.
   I'll still need to complete the entire tutorial later to really learn it.

2. But, reading that full tutorial will not make me a real javascript programmer.
   So I figure I would need to actually learn Javascript first.
   This [Q&A](https://www.quora.com/Do-i-need-to-study-JavaScript-in-order-to-study-Angular-js)
   also mentions [same philosophy](http://snipcart.com/blog/learn-vanilla-javascript-before-using-js-frameworks).

3. The implementation based on Angular is very concise,
   largely because it is not needed to explicitly define cell IDs and their listeners.
   But, to be fair, later I figure we could probably also implement a jQuery-based version
   which defines a global listener on all cells,
   and changes their style on-the-spot without needing to define cell IDs either.
   But at least the Angular way forces me to do it in the concise way from the beginning,
   which is not a bad thing.

I may continue to update this project during my learning process on javascript.

