# Why mathematics

## Excercises

1. A wolf, a goat, and a cabbage are to be rowed across a river in a boat holding only one of these three objects besides the oarsman. How should he carry them across so that the goat should not eat the cabbage or the wolf devour the goat?

2. A man goes to a tub of water with two jars, one holding 3 pt and ther other 5 pt. How can he bring back exactly 4 pts?

3. Two husbands and two wives have to cross a river in a boat which can hold only two people. How can they cross so that no woman is in the company of man unless her husband is also present?

### Wolf, goat, cabbage

My guess was to carry goat to the next shore by the first time, but then I stucked into an idea that I cannot bring no wolf to the goat, nor cabbage. My fail was in the assumption that the sailsman cannot bring something to another shore simultaneously to taking back an object already staying on the shore.

So, my algorithm was incomplete:

0. wolf, goat, cabbage
1. take goat to another shore
2. ?

While the right answer is:

0. wolf, goat, cabbage
1. take the goat to another shore
2. sail back in empty boat
3. take the cabbage to another shore
4. leave the cabbage and take the goat back
5. leave the goat and transfer the wolf to the cabbage
6. leave the wolf with the cabbage and sail back empty
7. take the goat to another shore where the wolf is bored


### 2 jars of 5 and 3 pt

My first idea was to full 5 pt one and then pour 3 pts to another one leaving 2 pts in the first. Then, I thought, I should empty the 3 pt jar leaving 2 pts in 5 pt jar but there is no next step.

The next algorithm emerged from an equation `4 = (5 + 3) / 2` that brought me a guess that a man can full both jars, then half each of them and then combine both of them in one volume getting 4 pts as a result. This sounds correct but I missed the point that no one can precisely empty the jar, thus the answer is incorrect.

The correct one is based on the even simpler equation `4 = 5 - 1` or, in terms of 5 and 3 pt jars, `4 = 5 - (3 - 2)`, where 5 is a 5 pt jar, 3 is a 3 pt jar and 2 is a 5 pt jar subtracted 3 pts of water. The correct answer is:

1. full 5pt jar
2. leave 2pt by pouring 3pt from it
3. full 5pt jar again
4. fill 3pt with lacking 1pt, which will leave exactly 4pt in 5pt jar


### Two husbands and two wives

My algorithm was a literal analogy of the first problem solution.

Say the guys are named Mr and Mrs A, and Mr and Mrs B.

1. Mr A + Mrs A to the right
2. Mr A back
3. Mr A + Mr B to the right
4. Mr A + Mrs A back, Mr B is left
5. Mrs A + Mrs B to the right, Mr A is left on the first shore
6. Mrs B is left with Mr B on the right
7. Mrs A travels back
8. Mrs A + Mr A travel right

This is a working solution but not the optimal one. The best is simpler:

1. Mr A + Mrs A ->
2. Mr A returns
3. Mr A + Mr B ->
4. Mrs A returns
5. Mrs A + Mrs B ->

My fail was to accept the first working solution. I think the correct approach is to _start_ with any working one and then develop it into a simpler one.

Maybe the next generation of thinking is to make a model representing the problem first, and then to develop it.