Imagine that I offer you the following game.  

First, you pay a sum of money to play the game.  

I toss a coin.  If it comes up heads, I pay you £2.  
If it comes up tails, I toss again.  If it comes up heads, I pay you double the previous prize which in this case is £2 * 2 = £4.
  
Essentially the entire game is a loop:

Set the prize to be £2
Repeat:
Toss the coin
If it comes up tails, double the prize  
Until – it comes up heads 
Pay out the prize.
  
The paradox arises because the overall expected payoff is the sum of the individual expected payoffs, all of which are £1 (see the lecture notes).  The number of individual expected payoffs is infinite.  So there should be no limit to the amount that you would be willing to pay in order to play.  In practice you would be very foolish to do so.  

One question we never discussed was “What is, in practice, a reasonable amount to pay to play?”  If you offer to pay £1 to pay, you are clearly going to win every time.  If you pay £2 to play you will break even 50% of the time and make a profit 50% of the time. So, at least £2 is a safe bet.  

But what about larger amounts?  

For example, suppose you decide to pay £5 to play.  If you play 10 games do you, on average, win?  If you play 20 games do you, on average, win?  If you increase the number of games you are prepared to play, does that increase or decrease your chances of winning? 

One way to try to answer this is with a MCS.  

Let’s stick with £5 to play for a moment.  If you play 10 games it will cost you £50 to play them all.  If your winnings exceed £50 you have made a profit, if they are less than £50 you have made a loss.

But if you played another 10 games, your winnings/loses are likely to be different because each game has a random element.  But that is OK because this is a MCS.  So you can program it to play 10 games over and over again until you have enough results to average them and get a good, reliable, answer.  This will tell you whether, on average, a bet of £5 and playing 10 games is going to be profitable (or not).

But, of course, you could do this again for 20 games and 30 and a whole host of other numbers of games whilst keeping the same pay to play (£5 per game).  

And, of course, you can also investigate what happens if you vary the amount you are prepared to pay to play.  In other words, you can create a two-dimensional matrix like this:




Pay	 	Average	 	 
to 	 	Number of games played	 	 
Play	1	2	3	etc.
£1	 	 	 	 
£2	 	 	 	 
£3	 	 	 	 
£4	 	 	 	 
etc.	 	 	 	 


In the cells at the intersection of these two values, you can put the average gain or lose that you have calculated.  

So the assignment is to write a MCS in R that provides the data to fill this matrix.  We leave it up to you to decide which:
pay to play values you investigate
average number of games you try
the number times you run the MCS with a given number of games.
