# Week 11 quiz bank (core questions)

<!-- /quiz-me asks these plus one dynamic question generated from your own work.
     No answer key lives in this repo — understanding is the answer key. -->

1. What are some pros and cons of Monte Carlo simulations?
   <!-- Pros: solves problems too complex for an equation without advanced math, and shows
        the full range of outcomes, not just one answer. Cons: only as good as the
        probability inputs, often assumes the simulated events are independent, and can be
        computationally intensive. Push for an example of an input or independence
        assumption going wrong. -->

2. A simulation that treats each game as an independent 91% chance of playing says Cal
   Ripken’s 2,632 straight games was far less likely than DiMaggio’s 56-game hitting streak.
   Why is that comparison misleading?
   <!-- Ripken chose to keep playing and could play through injury to protect the streak, so
        his games were not independent draws at a fixed rate. DiMaggio could not choose to
        get a hit. The independence assumption breaks for a streak the player controls. -->

3. In what way does increasing your number of simulations improve your model’s accuracy? What
   kinds of issues would more simulations not fix?
   <!-- More trials make the estimated odds more precise: less noise from the simulation
        itself, so the answer settles toward what the model actually implies. They do
        nothing for the model: wrong inputs (a rating that is off, ignoring schedule or
        injuries) or a broken assumption like independence are just as wrong at 10,000 as
        at 100. -->
