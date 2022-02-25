---
layout: page
title: Point Systems
permalink: /point-systems
nav_order: 10
has_children: false
---

<script type="text/javascript" src="https://unpkg.com/mermaid@8.0.0-rc.8/dist/mermaid.min.js"></script>
<script>$(document).ready(function() {mermaid.initialize({theme: 'forest'});});</script>

Point System Design
================================
The PlastiPoint system can be thought of as a "Non-Fungible" point reward system built upon a gamification framework of services. The three main components are:
1. Chart of Weight to Point Conversions
2. Chart of Services and Costs
3. Redemption Chart of Points to Rewards

There are many external forces on the system including: demographics, regionality, market forces and reward liquidity. Before we dive more in depth on how the system works lets first examine some popular point systems that exist today.


Background on Point Systems 
---------------------------

Many point systems exist today including: 
-  Credit Card dividends
-  Airline loyalty points
-  Grocery store cards (or entering  a phone number at checkout)
-  Junk mail coupons

<div class="mermaid">
graph TD;
    Coupon;
    Airline-Miles;
    Dividends;
</div>

These are all examples of different point systems.

Point systems can get complex, sometimes even morphing a companies traditional business 
model away from the core service they offer and making them act more as a sudo-bank or finance company. This video does a good job explaining the complexaties of a point system: "How Airlines Quietly Became Banks" <a href="https://www.youtube.com/watch?v=ggUduBmvQ_4" target="_blank">https://www.youtube.com/watch?v=ggUduBmvQ_4</a>

**Dividends**
Many systems include dividends to incentivise certain consumer behavior. Citicard has a dividend that incentivises 
users to use their credit card over competitors cards. Users typically get 1-5% percent cash back on purchases made. Then after a 
certain amount of time when they hit a threshhold, let say $300, they can request a check. The hidden reason is Citi wants more customers. 
More customers means more profit from two sources (1) from users that hold a balance and paying interest rates (2) from fees harvested 
from the visa/mastercard network. At the end of the day the consumer ends up footing the bill. They are tricked into thinking they got 
a free lunch (via the dividend) when in reality the fee is passed back them in the price of consumer goods from retailers and businesses 
that have to pay a fee to use the network. 


**Airline Miles**
Airlines have a miles reward system. Typically the incentive is for you to exclusivley fly a certain airline to earn loyalty points and 
bundle with a car rental and credit card company. The consumer may think they are racking up points and getting free vacations but most 
of the time they are choosing slightly more expensive flights throughout the year to earn the points (probably because their employer 
is footing the bill). These points are not tranferable between airlines and lock the consumer into one vendor. In recent times, many of the large
airlines have had their reward systems valued higher than the core business on the stock exchange. 

The PlastiPoint reward system is slightly different. The devil is in the details. 

To get into the details we must define two finance terms (1) fungible tokens and (2) non-fungible tokens. 
These are just fancy words for different types of "Points".

Fungible Token
----------------
- Example: Currency
- Every unit is worth the same value
- Easily divisible. 1 dollar can be split into (4) 25 cent quarters
- Tranferrable

Non-Fungible Token
------------------
- Example: A token representing something physical (digital twin)
- Example: A collectible like a baseball card
- Transferable value associated to the transaction
- Typically it's hard to put a global value on the unit. The value derives from the the eye of the beholder or system
- Programmable
- Can add metadata to the token, such as GPS location or date aquired
- Certifiable: can prove its recycled
- Traceable: can trace from consumer to recyling center to reuser etc...

The PlastiPoint 
-----------------
The PlastiPoint is a non fungible point and reward system built upon a gamification framework. Demographics, regionality, market forces and reward liquidity effect the system. The system is much more complicated than a simple static point to cash exchange rate. It depends heavily on consumer core drives, cost to move the material, and the market value of the material (which changes daily).

The idea
--------
The big idea is to split the point system into three logical charts: 
- (1) Chart of Weight to Point Conversion
- (2) Chart of Services and Costs 
- (3) Chart of Points to Reward (Redemption/Exchange)


(1) Chart of Weight to Point Conversions
-----------------------------------------

|  KG   |  Points |
| ----- | ------- |
|   1   |   100   |
|   2   |   200   |
|  ..   |   ...   |
|  10   |  1000   |

- The chart above represents the "PlastiPoint Standard". It's a global standard that pegs the weight in kilograms to how many points 
are rewarded to a consumer for recycling. This chart is system wide and should never change.
- I propose we use the the conversion above (1KG = 100 Points). In the future somebody might invent a machine that allows a consumer to take back a single lightweight flexible packaging material, for example, a plastic wrap from a food item. The item might only weigh 1 gram. We simply do the math and award the user 0.1 points. 

(2) Chart of Services and Costs
----------------------------------

|       Service                  |      Cost     | Demographic     | Incentive     |    KG    | Points Earned  |   Subsidy Paid to Consumer     |  Material Value Split % Paid 2 Consumer | Premium Features        
| ------------------------------ | ------------- | --------------- | ------------- | -------- | -------------- | ------------------------------ | --------------------------------------  | ----------------------------------------
|     Residential Pickup (Paid)  |  300 KSH      |  High Income    | convenience   |     1    |     100        |      0                         |     0%                                  | On Demand Pickup in AM or PM 
|     Residential Pickup (Paid)  |  350 KSH      |  High Income    | convenience   |     2    |     200        |      0                         |     0%                                  | On Demand Pickup in AM or PM 
|     Residential Pickup (Free)  |    0 KSH      |  Medium Income  | convenience   |     1    |     100        |      0                         |     0%                                  | Flexible Pickup whenever an efficient route is available
|     Drop Off (Subsidized)      |    0 KSH      |  Low Income     | point reward/cash |  1   |     100        |     100 KSH                    |     5%                                  | N/A
|     Drop Off (Unsubsidized)    |    0 KSH      |  Medium Income  | point reward   |     1   |     100        |      0                         |     7%                                  | N/A

- <i>Most of the values above are dynamic...except "KG to Points"</i>

- `Services` 
    - The "Residential Pickup (Paid)" service offers a premium "On Demand Pickup" feature
    - The "Residential Pickup (Free)" service offers a non time sensative pickup window
    - the "Drop off" service offers the consumer getting a reward/paid   

- `Demographics` The chart above shows specially crafted services for different demographics. 
There are many different types of users in the system with different desires driving their actions. 
Lets take, for example, the three types of consumers: High Income Consumer, Low Income Consumer and Medium Income consumer. The high income consumer may 
be willing to pay 300 shillings to a collector for a residential pickup. This is based on a convenience factor, which can be thought of 
as a premium feature.  In return, they may want to document this act of goodwill. We could in return give them a certain amount of points 
in return for the effort (they could possibly donate the reward). 

- `Incentives` The goal is to figure out what the minimum reward is to drive recycling behaviors. The 
complexity above can be hidden in the app. As time goes on and we build out the network we may be able to offer free residential 
pickups. I think this goal ought to be thought more of as a means of gamification and avoid getting stuck with details of 
exchange rates (at the consumer level). 

- `Subsidies` Some demographics will need to be paid to recycle, specifically the `drop off` service targeting the low income demographic. 
This could be in the form of donations from sponsors, governments, or possibly a dividend cut from the local recycling center.

- `Material Split` When a consumer drops off recycling at a center they could get a percentage of the value. This will be based on
many market factors, as well as how efficient the local recycling system is. I suspect at first the split for the consumer will be 0% but in 
time as the recycling supply chain becomes more effiecnet and the value of the material increases the material split could increase and consumers
could get paid to recycle!

- `Gamification` All the factors above can be addressed by a gamification framework. A framework called the "Octalysis framework"
is used by all major tech companies from Uber to Google. In "big tech" some services appear to be free but they have different business models backing them. 
<a href="https://yukaichou.com/gamification-examples/octalysis-complete-gamification-framework/" target="_blank">https://yukaichou.com/gamification-examples/octalysis-complete-gamification-framework/</a>
 
(3) Redemption Chart of Points to Rewards
------------------------------------------

|   Points    |   Reward                                  | Reward Sponsor      | Redeemable Location |  Date    | 
| ----------- | ----------------------------------------- | ------------------  |  ------------------ | -------- | 
|     1000    |   50 KSH discount on Coke at Total        |   Coke              |       Nairobi       |  2/22/22 | 
|     800     |   50 minutes of Safaricom Talk/MSG/ect... |   System - bulk buy | Nairobi             |  2/22/22 | 
|     500     |   Give as gift to collector/friend/etc... |   System - transfer | Nairobi             |  2/22/22 | 

- When you want to exchange your points for rewards there are several determining factors that effect the exchange rate. 
    1. The value of the material at that point in time.
    2. How many rewards are in the system (Reward Liquidity)
    3. Your physical location. 
- The factors above mean the exchange rates are dynamic.
- Exchaning points for rewards can be location specific. For example, coupons may only be redeemable in certain cities and states.
Since each point is a "non fungible token" we can enforce location based contraints (geofence) becuase we save metadata about location with each point.
- Rewards are for both high income demographics and low income. High income earner may choose donation based rewards over products.
- To successfully bootstrap the rewards program we need to build a network of reward sponsors and integrate into existing systems like, coupon/discount/gift card/point-of-sale systems.
Buying rewards in bulk at a discounted rate could help bootstrap the rewards system, see https://africastalking.com/airtime
- We also need to make sure we maintain a healthy pool of rewards to keep consumers engaged. Possibly, in low reward liquidity times, we could resort to digital rewards and games.
- In time, game theory suggests the value of the material will increase making the system less and less dependent upon reward sponsors and more 
incentives could come from the "material value split".


Q: Why would a company, like Coke, want to become a rewards sponsor? 
--------------------
1. `To meet sustainability goals`
Each point in the system represents weight in KG of material being recycled and taken out of the environment.
The PlastiPoint is proof of recyling...in other words its a certificate. Often times credit systems, such as Carbon Credits are hard to audit and even harder to provide tangible metrics of environmental improvements. Solid objects, like plastic are much easier to provide metrics for. The PlastiPoint is physcial proof that can be audited to prove something was actaully recycled. With these proofs in place a company could use that for meeting their sustainabilty goals.
2. `To market a new product`
The app will eventually have a large user base which will make a great marketing platfrom to promote new products.
3. `To drive complementary purchases`
If a user walks into a Total convenience store with a coupon to buy Coke they might also make complementary services at the store. 

Revenue Opportunites
------------------------------
As the user base grows the revenue opportunies grow. There will be more sponsors coming on board to sell ads to or bump their product up for 
premium "billboard" space in the rewards store.

The Goal
--------
The goal is to create a global efficient system and incentivise competition to drive the value of the material up (used in more products) 
and drive down the cost of labor and the cost to produce/transport the material. A good goal to shoot towards is to not even use rewards or subsidies and make 
the value split of the material pay for the service itself...creating a self-sustaining system.


<div class="mermaid">
graph TD;
    consumer-->collector;
    collector-->recycler;
    recycler-->exchange;
    exchange-->reuser;
    reuser-->consumer;
</div>