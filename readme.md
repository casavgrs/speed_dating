# Speed Dating experiment - the difference in behavior and perception by gender and race from an Asian Male's perspective
## by Kazu Fukuda


## Dataset

I analyze Speed Dating experiment dataset on Kaggle(https://www.kaggle.com/annavictoria/speed-dating-experiment) that consists of the individual choices of people when selecting their dates in the speed dating environment by Columbia graduate school students. <br>

In the experiment, each participant fills out their biological information.<br> 
In each session, participants rated partners based on the following criteria on a scale of 1-10:<br> 
1) Attractiveness, 2) Sincere, 3) Intelligent ,4) Fun, 5) Ambitious, 6) Shared interests,7) Overall like( willingness to date the partner of the session)<br>
Participants attended speed dating events and conducted 4,174 sessions.<br>
After rating their partner, they decide whether they want to see the partner again(decision). When both of them want to see each other again, then they are “matched” and they can exchange their phone numbers.<br>

##### [Id]
**`iid`**: Participant's ID<br>
**`pid`**: Partner's ID<br>

##### [Gender]
**`gender`**:	Female=0, Male=1 <br>

##### [Race]
**`race`**:Black/African American=1, European/Caucasian American=2,Latino/Hispanic American=3,Asian/Pacific Islander/Asian-American=4,Native American=5, Other=6 <br>
**`race_o`**:Race of partner<br>
**`samerace`**:Partner is the same race 1=yes, 0=no<br>

##### [Decision]
**`dec`** Decision of a session 1=yes, 0=no <br>
**`dec_o`** Partner's decision of a session 1=yes, 0=no  <br>

##### [Rating]
**`like_o`** Overall, how much do you like this person?(1=don't like at all, 10=like a lot)<br>
**`attr_o`** Attractive rating of partner(1=awful, 10=great)<br>
**`sinc_o`** Sincere rating of partner(1=awful, 10=great)<br>
**`intel_o`** Intelligent rating of partner(1=awful, 10=great)<br>
**`fun_o`** Fun rating of partner(1=awful, 10=great)<br>
**`amb_o`** Ambitious rating of partner(1=awful, 10=great)<br>
**`shar_o`** Shared Interests/Hobbies rating of partner(1=awful, 10=great)<br>


## Summary of Findings

#### The probability of being selected and the mean rating received from and given to their partners 

- The distribution of the probability of being selected is right-skew for both males and females, and there is no significant observed difference for both gender.<br>
- As for the mean rating given to their partners, it is interesting that the distribution of males is more widely spread(standard deviation:0.94) whereas the distribution of females is sharper(standard deviation:0.79).


#### The males' probability of being selected from females in difference races
- The distribution of the males' probability of being selected by females are all right-skewed.
- The Asian Males' probability of being chosen by females(7%) is lower than that of non-Asian(10%)(P-value:0%)

#### The males' mean rating score received  from females in difference races
- The Asian Males' mean rating received by females(6.1) is lower than that of non-Asian(6.3)(P-value:0%) (P-value:1%)

#### The rating attributes and Asian Males' likelihood of being selected by Asian and White females(two major races at the experiment)
- All the VIF factors of the attributes are less than 5. Thus, there is not significant multicollinearity among attributes
- There is no attribute that has a higher coefficient for white females. However, as for Asian Females, sincere and intellectual have a higher coefficient than other attributes.
- Attractive rating and the decision of the partner is negatively correlated


## List of resources used
Speed Dating experiment dataset on Kaggle(https://www.kaggle.com/annavictoria/speed-dating-experiment) 
