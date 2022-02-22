---
layout: page
title: Point Systems
permalink: /point-systems
nav_order: 10
has_children: false
---

<script type="text/javascript" src="https://unpkg.com/mermaid@8.0.0-rc.8/dist/mermaid.min.js"></script>
<script>$(document).ready(function() {mermaid.initialize({theme: 'forest'});});</script>

PlastiPoint Gamification System
================================
The PlastiPoint can be thought of as a "Non-Fungible" reward system built upon a gamification framework. Demographics, regionality, 
market forces and reward liquitity all effect the system. More on the explaination of this below but first lets examine some popular 
point systems that exist today.


Background on Point Systems 
---------------------------

Many point system exists today including: 
-  Credit Card dividends
-  Airline loyalty points
-  Grocery store cards (or entering  a phone number at checkout)
-  Junk mail coupons

<div class="mermaid">
graph TD;
    Coupon;
    AirlineMiles;
    Dividends;
</div>

These are all examples of different point systems.

This video does a good job explaining the complexaties of a point system....sometimes even morphing a companies traditional business 
model away from the core service and acting more as a sudo-bank or finance company. Watch: How Airlines Quietly Became Banks 
<a href="https://www.youtube.com/watch?v=ggUduBmvQ_4" target="_blank">https://www.youtube.com/watch?v=ggUduBmvQ_4</a>

**Dividends**
Many systems have dividends or rewards systems to incentivise certain consumer behavior. Citicard has a dividend that incentivises 
users to use their credit card over competitors cards. Users typically get 1-5% percent cash back on purchases made. Then after a 
certain amount of time when they hit a threshhold, let say $300, they can request a check. The hidden reason is citi wants more customers, 
more customers means more profit from two sources (1) from users that hold a balance and paying interest rates (2) from fees harvested 
from the visa/mastercard network. At the end of the day the consumer ends up footing the bill. They are tricked into thinking they got 
a free lunch (via the dividend) when in reality the fee is passed back them in the price of consumer goods from retailers and businesses 
that have to pay a fee to use the network. 


**Airline Miles**
Airlines have a miles rewards system. Typically the incentive is for you to exclusivley fly a certain airline to earn loyalty points and 
bundle with a car rental and credit card company. The consumer may think they are racking up points and getting free vacations but most 
of the time they are choosing slightly more expensive flights throughout the year to earn the points (probably because their employer 
is footing the bill). These points are not tranferable between airlines and lock the consumer into one vendor.

The PlastiPoint reward system is slightly differnet and the devil is in the details. 

To get into the details we must define two finance terms (1) fungible tokens and (2) non-fungible tokens. 
These are fancy words for different types of "Points".

Fungible Token
----------------
- Example - Currency
- Every unit is worth that same value
- Easily divided and divisible. 1 dollar can be split into (4) 25 cent quarters
- Tranferrable

Non-Fungible Token
------------------
- Example - A token representing something physical (digital twin)
- Example - A collectible like a baseball card
- It's hard to put a global agreeable value on the unit, the value dervices from the the eye of the beholder.
- Programmable
- Transferrable
- Can add metadata to the token, such as GPS location or date aquired
- Certificable - can prove its recycled
- Traceable - can trace from consumer to recyling center to reuser etc...

The PlastiPoint 
-----------------
The PlastiPoint is a non fungible point and reward system built upon a gamification framework. Demographics, regionality,
market forces and reward liquitity all effect the system.

The idea
--------
The idea is to split the point system into three logical charts: 
- (1) Chart of Weight to Points
- (2) Chart of Services and Costs 
- (3) Chart of Points to Reward (Exchange)

The system is not just a simple static point to cash exchange rate. It depends heavily on consumer demographic, core drives, 
cost to move the material, and market value of the material (which changes daily).

1. Chart of Weight to Points
- |  KG   |  Points |
  | ----- | ------- |
  |   1   |   100   |
  |   2   |   200   |
  |  ..   |   ...   |
  |  10   |  1000   |
- The chart above represents the "PlastiPoint Standard". It's a global standard that pegs the weight in kilograms to how many points 
are rewarded to a consumer for recycling. This chart is system wide and should never change.
- I propose we use the the conversion above (1KG = 100 Points). In the future somebody might invent a machine that allows a consumer to take back
one lightweight flexible packagaing materiak (let's say a plastic wrap for a food item). The item might only weight 1 gram. We simply do the math and award the user 0.1 points. 

2. Chart of Services and Costs
    
    - | Demographic     | Incentive     |       Service                  |      KG     | Points Earned |   Subsidy Paid to Consumer    |  Amount Owed  |  Material Value Split % Paid 2 Consumer | Premium Features        
      | --------------- | ------------- | ------------------------------ |  ---------  | ------------- | ----------------------------- | ------------- | --------------------------------------  | ----------------------------------------
      |  High Income    | convenience   |     Residential Pickup (Paid)  |      1      |     10        |      0                         |  300 KSH      |     0%                                  | On Demand Pickup in AM or PM 
      |  High Income    | convenience   |     Residential Pickup (Paid)  |      2      |     20        |      0                         |  350 KSH      |     0%                                  | On Demand Pickup in AM or PM 
      |  Medium Income  | convenience   |     Residential Pickup (Free)  |      1      |     10        |      0                         |    0 KSH      |     0%                                  | Flexible Pickup whenever an efficient route is available
      |  Low Income     | reward        |     Drop Off                   |      1      |     10        |     100 KSH                    |    0 KSH      |     5%                                  | N/A
    
    - The chart above shows specially crafted services for different demographics. There are many different types of users in the system with different desires driving their actions. 
    Lets take, for example, the three types of consumers: High Income Consumer, Low Income Consumer and Medium Income consumer. The high income consumer may 
    be willing to pay 300 shillings to a collector for a residential pickup. This is based on a convenience factor, which can be thought of 
    as a premium feature.  In return, they may want to document this act of goodwill. We could in return give them a certain amount of points 
    in return for the effort (they could possibly donate the reward). Lets assume the following "Chart of Services and Costs":
    
    - The goal is to split the demographic and figure out what the minimum amount of reward is to drive recycling behaviors. The 
    complexity above can be hidden in the app. As time goes on and we build out the network we may be able to offer free residential 
    pickups. I think this goal ought to be thought more of as a means of gamification and not to get stuck on the details of 
    exchange rates (at the consumer level). 
    
    - In regards to raising funds for the subsities for the low income services we can look into a really popular Gamification review the Octalysis framework.
    This framework is used by all major tech companies from Uber to Google. In "big tech" some services appear to be free but they have different business models
    backing them. 
    https://yukaichou.com/gamification-examples/octalysis-complete-gamification-framework/ 
 
3. Points to Rewards Exchange
    - When you want to exchange your points for rewards there are several determining factors that effect the exchange rate. 
        1. The value of the material at that point in time.
        2. How many rewards are in the system (Reward Liquidity)
        3. Your physical location. 
    - The factors above mean the exchange rates are dynamic.
    - Exchaning points for rewards can be location specific. For example, coupons may only be redeemable in certain cities and states.
    Since each point is a "non fungible token" we can enforce location based contraints (geofence) becuase we save metadata about location with each point.
    - Rewards are for both high income demographics and low income. High income earner may choose donation based rewards over products.
    - A example exchange chart could look like this:
    - |  Location  |     Date     |   Points    |   Reward                                  | Reward Sponsor
      | ---------- | -----------  | ----------- | ----------------------------------------- | --------------
      | Nairobi    |      2/22/22 |     1000    |   50 shillings discount on Coke at Total  |   Coke
      | Nairobi    |      2/22/22 |     800     |   50 minutes of Safaricom Talk/MSG/ect... |   System (buying in bulk - see https://africastalking.com/airtime)
      | Nairobi    |      2/22/22 |     500     |   Give as gift to collector/friend/etc... |   System txn
    - To successfully bootstrap the program we need to work and build a network of reward sponsors and integrate into existing coupon/discount/gift card/point-of-sale systems.
    - We also need to make sure we maintain a healthy pool of rewards to keep consumers engaged. Possibly, in low reward liquidity times, we could resort to digital rewards and games.
    - In time, game theory suggests the value of the material will increase making the system less and less dependent upon reward sponsors and more 
    funding could come from "material value split".


The Goal
--------
The goal is to create a global effiecient system and incentivise competition to drive the value of the material up (used in more products) 
and drive the cost of labor to produce and transport the material down. A good goal to shoot towards is to not even use reward or subsidies and make 
the value split of the material pay for the service iteself.


<div class="mermaid">
graph TD;
    consumer-->collector;
    collector-->recycler;
    recycler-->exchange;
    exchange-->reuser;
    reuser-->consumer;
</div>