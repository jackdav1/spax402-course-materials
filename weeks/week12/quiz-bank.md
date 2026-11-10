# Week 12 quiz bank (core questions)

<!-- /quiz-me asks these plus one dynamic question generated from your own work.
     No answer key lives in this repo — understanding is the answer key. -->

1. What is overfitting? How does a train/test split help you catch it?
   <!-- A model that fits the data it learned from so closely that it memorizes noise, and
        does worse on new data. Judge it on rows it never saw: a big gap between training and
        test accuracy is the sign. The called-strike tree with no depth limit was right on
        100% of training pitches and about 90% of new ones. -->

2. A model predicts whether a field goal is good and is right 85% of the time. Why might that
   model still be useless?
   <!-- About 85% of field goals are good, so a model that says every kick is good is right
        85% of the time and never catches a miss. Compare with that baseline, and look at the
        confusion matrix, not accuracy alone. -->

3. What is data leakage? Give a sports example of a column that would leak into a model.
   <!-- Using information the model would not have when it makes the prediction, so it looks
        better than it can ever perform. Examples: the count after the pitch in a called-strike
        model, opponents' full-season win percentage when predicting the second half (Week 5),
        how a drive ended when predicting a play in the middle of it. Push for why it inflates
        accuracy, and how they would catch it: ask when each column becomes known. -->

4. When would you optimize for recall instead of precision? Give an example from sports.
   <!-- Recall when missing a real positive is the costly mistake (a screening test, flagging
        an athlete at risk); precision when a false alarm is the costly mistake (spam,
        benching a player on a false flag). Their example should name which error costs more
        and to whom. -->

5. How is a random forest different from a single decision tree, and why does it usually do
   better on new data?
   <!-- Many trees, each grown on a random sample of the rows and considering a random subset
        of columns at each split, voting. Each tree overfits in its own way, and the vote
        averages much of that out. The cost is a model you can't draw as one set of rules. -->

6. What is a false positive in a model that predicts called strikes? What is a false negative?
   <!-- With strike as the positive class: a false positive is a pitch the model calls a
        strike that the umpire called a ball (Type 1); a false negative is a pitch the model
        calls a ball that the umpire called a strike (Type 2). -->
