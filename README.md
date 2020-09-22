# Mentorship
You can visit my created website [here](https://proxp.netlify.app/)
## Data Analytics
User Behavior Analytics or UBA focuses on what the user is doing: apps
launched, network activity, and, most critically, files accessed (when the file or
email was touched, who touched it, what was done with it and how frequently). <br>
UBA technology searches for patterns of usage that indicate unusual or
anomalous behavior — regardless of whether the activities are coming from a
hacker, insider, or even malware or other processes. While UBA won’t prevent
hackers or insiders from getting into your system, it can quickly spot their work
and minimize damage.<br>
I have integrated my website to an analytics platform named Google Analytics.
This tool is able to track the users action and the time spent by the users on the
various actions of the website. I have accumulated the analytics data from
various users and stored it.<br>
I have collected data of around 102 users with various data points such as: <br>
● Time spent by users on the different pages on website,<br>
● Filters being used by the users , <br>
● Time spent by users on a particular product page, etc.

## ML Model
The elusive clickstream data. Many platforms, like Facebook rely on these
generated data from what a user clicks and what doesn’t. To start analyzing
clickstream data, we need first to be able to capture step by step a user’s activity
across a web page or application. And that is of great value in the hands of any
Internet marketer. Getting a 360-degree view of a customer by knowing what he
is clicking and what he is not can get you a huge improvement in both your
products and your customers’ experience.
<br>
### Data Collection
Either you have your data in your data warehouse, or you need to enrich it with
more data sources you need to have a way to collect and store data consistently
into a database. <br>
### Data Preparation
Raw data is like a rough diamond; It requires some refinement before being truly
valuable. <br>
In the data world, refinement includes data processing, cleaning, and
transformation of the initial data into something convenient for the analysis you
are going to carry out. <br>
In this case, we would like to have our data grouped into users. It would be
good too, we could arrange the events of each user in time order before moving
to actual analysis. <br>
In contrast to other data sequences, clickstream data can have varying
length for every different user. <br>
In order to transform the initially collected event log into clickstream data
we need to: <br>
★ Identify events/actions performed by the same user and group them
together <br>
★ Split them further into subgroups of events based on which of those were
performed during the same session according to the session’s definition
given above. <br>

### Model Construction
As in most cases, the methods we can deploy for solving this problem are many. <br>
### Markov Chains
The type of data Markov Chains work with are sequential data. <br>
The Markov process is a stochastic process that satisfies the Markov
Property of memorylessness. A Markov chain is, in fact, a Markov process too in
either discrete or continuous time with a countable state space.<br>
In clickstream analysis, we usually utilize these Markov Chains. The
process takes the state from a finite set at each time . The order of a Markov
Chain is derived from the number of recent states on which the current state, we
assume, depends. Based on this, zero-order chains imply that the probability of
being in a state in the next step is independent of all previous states.<br>
Higher order Markov Chain introduced by the Raftery (1985) will lead to
more realistic models. At the same time, the parameters needed for the
representation increase exponentially and so it is important to find a right balance
between these two. <br>
### Fitting a Markov Chain
Fitting the Markov Chain model gives us the transition probabilities matrices and
the lambda parameters of the chain for each one of the three lags along with the
Start and End Probabilities.
Start and End probabilities correspond to the probability that a clickstream will
start or end with this specific event.
The transition probability matrix can be represented as a heat map with the
y-axis representing the current state and x-axis the next one. The more blueish
the color, the more probable the indicated transition will occur.
<br>
![Heat Map!](https://github.com/HeeteshSimon/Mentorship/blob/master/Heat-Map.png)
![Graph!](https://github.com/HeeteshSimon/Mentorship/blob/master/round-table.gv_page-0001.jpg)
