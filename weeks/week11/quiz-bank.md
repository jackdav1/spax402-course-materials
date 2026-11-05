# Week 11 quiz bank (core questions)

<!-- /quiz-me asks these plus one dynamic question generated from your own work.
     No answer key lives in this repo — understanding is the answer key. -->

1. What does a Monte Carlo simulation do, and what do you have to decide before you can run
   one?
   <!-- Runs many random trials of an uncertain process and counts how often each outcome
        happens. You choose the chance of each small event (a goal in a minute, a team
        winning a game). The answer is only as good as those inputs. -->

2. A simulation says a team down one goal should pull its goalie with about five minutes left.
   Which inputs would have to change for that answer to move later?
   <!-- The scoring rates: if the extra attacker adds less scoring, or the other team hits
        the empty net more often, the best pull time moves later. Push for "the rates," not
        "run more simulations." -->

3. A simulation that treats each game as an independent 91% chance of playing says Cal
   Ripken's 2,632 straight games was far less likely than DiMaggio's 56-game hitting streak.
   Why is that comparison misleading?
   <!-- Ripken chose to keep playing and could play through injury to protect the streak, so
        his games were not independent draws at a fixed rate. DiMaggio could not choose to
        get a hit. The independence assumption breaks for a streak the player controls. -->

4. Your simulation gives a team a 12% chance of making the playoffs, and they make it. Was the
   model wrong?
   <!-- Not on that evidence: 12% events happen about one time in eight. You judge a model
        on many predictions (did its 10% teams make it about 10% of the time), not one. -->

5. What do you gain by running 10,000 simulated seasons instead of 100, and what doesn't more
   simulations fix?
   <!-- More trials make the estimated odds more precise (less noise from the simulation
        itself). They do nothing for wrong inputs: a bad rating or a broken independence
        assumption is just as wrong at 10,000. -->
