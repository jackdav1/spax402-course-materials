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

4. When would you optimize for recall instead of precision? Give an example.
   <!-- Recall when missing a real positive is the costly mistake (a screening test, flagging
        an athlete at risk); precision when a false alarm is the costly mistake (spam,
        benching a player on a false flag). Their example should name which error costs more
        and to whom. -->

5. What is one advantage of a single decision tree over a random forest? What is one
   advantage of a random forest over a single decision tree?
   <!-- Tree: a coach can read it (a few yes or no questions you can draw and check), and it
        is cheap to train and run. Forest: it usually predicts better on new data because the
        vote averages out each tree's overfitting, and it gives a graded probability (the share
        of trees voting yes) instead of a deep tree's 0% or 100%. The cost is that you can't
        read 100 trees; you look inside with permutation importance instead. -->
