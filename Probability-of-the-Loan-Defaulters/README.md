### Project Overview

 One of the key responsibilities of a data scientist is to build systems that understand and interact with the real world. Real-world is filled with uncertainty - you cannot predict how certain events will turn out. When house owners in the USA defaulted on mortgages, the cascading effects led to the subprime housing crisis further leading to recession worldwide. Therefore, it is very important for a data scientist to model uncertainty.

Now, the next question is - how do we model uncertainty? While we cannot predict events accurately, we can form an idea of how likely the events will or will not occur. We often can't prove that something is true but we can ask how likely other events are or what is the most likely explanation. This kind of modeling is possible with probability.

The following image will give you a gist of the concept of probability you will learn along with the applications to data science. The application to data science will become clear as go through the course. But this would give you a sneak peek into the applications of probability to data science.
In particular, probability models uncertainty w.r.t time. Uncertainty in time corresponds to those events where the uncertainty is resolved with the passage of time. Think of the following questions:-

What will the weather be like in the morning?
What will be the price of the Microsoft stock tomorrow?
The uncertainty in these situations is resolved if we wait a certain amount of time. Once the morning passes, the uncertainty in weather is resolved. Once you watch the movie, you will know whether you liked the movie or not. And the next day will bring you the news regarding the price of your favorite stock.

Let's take the first example in the listed questions - What will the weather be like in the morning? To answer this question, the first thing we need to do is to ask ourselves what are the likely events that can occur. In this case, it is simple - rainy, sunny or cloudy. Only one of these events will occur. The events together form what is called a sample space.

Sample space is defined as the combination (set) of all possible outcomes.

For the first question, the sample space can be defined as
S={Sunny,Rainy,Cloudy}
S={Sunny,Rainy,Cloudy}

Similarly, for the second question, where we ask whether you will like the movie, the sample space can be defined as
S={Yes,No}
S={Yes,No}

For the third question, the sample space is not so straightforward. The stock could be at any value. Something disastrous could happen and the stock could fall to zero, or a great positive development could send the price skyrocketing. So the way to define the sample space is

S={x\ |\ x > 0}
S={x ∣ x>0}

Hence in order to define the sample space, we first need to formulate the questions that need answering. Asking the right questions is a crucial skill for a data scientist. Sample space can contain different types of data i.e. discrete, continuous or qualitative (categorical). We have learned how to summarize these different types of data in descriptive statistics. Here, we will learn how to answer uncertain questions regarding our data with the help of probability. It is time to define probability formally and explore it further.

**Problem Statement
**What is the probability that the borrower paid back their loan in full?

About the Dataset




### Approach taken to solve the problem

 After completing this project, you will have a better understanding of probability. In this project, you will apply the following concepts.

Independency check
Bayes theorem
Visualizing discrete variable
Visualizing continuous variable


### Additional pointers

 !!![container width="100%" align="center"]
![datset](undefined/account/b16/6a1f0c95-2915-474c-917f-dc711cc8d89b/b856/532d2d53-5133-403f-84e2-0ae35c10ccce/file.png)
!!![container-end]



