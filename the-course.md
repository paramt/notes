---
title: The Course notes
date: 2026-08-06
description:
unlisted: false
tags:
  - poker
rich: true
---
Notes from Ed Miller's [*The Course*](https://www.amazon.com/gp/product/1511768320?camp=1789&creative=9325&creativeASIN=1511768320&linkId=Z2QM344R5QTCFS55). WIP
# Part I: The 30,000 foot view
## The Many Forms of No-Limit Hold'em
- online is much tougher than live (live has more hobby players)
- everyone playing live poker at a casino is bad, don't listen to them
- it's easy for real skill to be masked by luck on a day-to-day basis: to be confident in your skills you need to be able to justify your decisions to yourself 

## Where Does The Money Come From
- from opponents who play too many hands. you must raise to fold better hands or get called by worse hands, to exploit players who play too many hands 
- by the river, most people actually play too few hands, even if they play too many hands preflop
- so you must know when to get out of the way, once your opponents have folded down to too few hands

Each skill is designed to ensure: 
1. you attack players when they play too many hands
2. you get out of the way when opponents strategies leave them with only strong hands 
3. you're not caught playing too many hands yourself 

  
# Part II: Beating Live 1-2 Games

## Skill #1: Play a Simple and Effective Pre-Flop Strategy
- hitting flops is not how you make money
- postflop, opponents strategies will vary a lot. but preflop, most opponents will play too many hands 
- play hands that have equity-when-called[^1] on a wide range of boards (showdown equity + fold equity) 
- these include suited cards that are either connected or are both big cards

suitedness is super valuable: 6% chance to hit a flush is a significant edge: 
- the hands you do hit a flush tend to let you win larger pots
- it gives you the opportunity to semi bluff with a draw because they have good equity-when-called

only enter a pot preflop by raising:
- raising bloats the pot, which compounds your opponents errors 
- it punishes people for playing too many hands 

### Early Position
Everything before BB, SB, BU, CO

#### Open (14%):
- 22+
- ATs+, KTs+, QTs+
- A2s-A9s
- JTs-76s
- AKo, AQo

Note that AKo and AQo are the only unsuited hands here

#### Facing a tight raise: 
3bet: AA, KK, A5s
Fold: AQo, A2s-A9s
Call: 22+, ATs+, KTs+, QTs+, JTs-76s, AKo

#### Facing a loose raise: 
3bet: AA-QQ, AK, A2s-A5s, T9s, 98s
Call: everything else in open range
  

### Cutoff 
#### Open (22%):
- 22+
- A2s+, K7s+, Q9s+
- 43s+
- 53s+
- ATo+, KJo+

#### Facing a tight raise: 
- same as EP facing a tight raise

#### Facing a loose raise: 
3bet: JJ+, AKs, A7s, A5s-A2s, T9s, 87s, 54s, AKo
Call: AQs-A8s, A6s, K9s+, Q9s+, JTs, 98s, 76-65s, J9s-86s, AQo-AJo, KQo

### Button 

#### Open (33%)
- 22+
- A2s+, K2s+
- Q5s+
- J7s+
- 43s+
- 53s+
- 96s+
- A7o+
- K9o+
- QTo+
- JTo


### Summary

1. play tight
2. avoid strength
3. attack weakness
4. dont try to make hands
5. choose hands that have equity-when-called
6. defend blinds against steals, not strong raises

essentially, play tight (play less hands, raise more) and avoid unsuited hands

  
  
  

### Multi-Way Pots and Loose Games

in games that are more loose and pots get big preflop, focus on hands that get there faster rather than take time to develop from draws (ie high cards over connectors) 
- can even add offsuit high cards and remove lower suited connectors




## Skill #2: Don't Pay People Off 

(big river bets)[^2] aren't bluffed enough (at low stakes), fold these 
- e.g. $100 raise into a pot of $100 => you can call 100 to win 200 => you need opponent to be bluffing 33% of the time to profitably call, opponents will not be bluffing with this frequency 
- they could bluff you off sometimes, but you can give it to them because frequency is not high enough

this doesn't apply to small bets or even raises -- opponents can bluff these easily (especially on the flop; people are more willing to bluff when there are more cards to come)

this is hard, especially if you have a good hand yourself. but it doesn't matter, if you're bluff catching, fold to a large river bet

it's ok to call the turn and fold the river, you're not committed and the river is a brand new decision 
- e.g. multiway pot where you have 4s4h, flop comes KsQs4c. you bet, get called. 
	- turn is Js completing straights and flushes. opponent bets 70 into a pot of 120. he's representing straight or flush. you can call, even knowing you're behind: 
		- you have 10 outs to a boat 
		- you might hit a baby flush and beat the opponent's straight
		- it's possible opponent has worse hands (like a two pair)
	- but once river bricks and opponent jams for 150 into a pot of 240, you should fold 
		- your outs missed 
		- if opponent had something like two pair, they would probably slow down after you called the turn bet
	- in general, this is new information: you didn't hit your outs and the opponent kept firing. both the turn call and river fold are justified

same principle preflop: opponents usually don't 3bet or 4bet light preflop. sometimes it's ok to call even knowing you're behind if stacks are deep. but usually ok to fold
### Multi-Way Pots and Loose Games
- in multiway, you can apply this fold logic to flop betting as well
	- if someone bets large into many people, it's usually very strong - can fold even top pair with a bad kicker

## Skill #3: Assess Your Hand Value
- when you flop a value hand, you don't want to push everyone out of the pot and win it now, you want to be paid off on all streets. this includes keeping the draws in, and sometimes getting outdrawn 
	- what happens if you get outdrawn? your opponents will tell you and you fold (Skill 2)
- ie you want to take good hands to showdown, not take it down immediately 
	- this doesn't work at higher stakes: good opponents are more willing to bluff, meaning you'll have to pay it off when they do outdraw you. at lower stakes, you can save the final bet because players don't bluff enough 
- when you flop a value hand, think about what worse hands will call you
- assess how many (streets of value)[^3] your hand has
	- TPTK[^4] usually has 2 streets of value (can change based on type of game/opponent, board texture -- especially on a (dynamic board)[^5])
- always have this plan: how many streets of value can you get (depending on how the board runs out), ie which worse hands will continue against you
- on top of how many streets of value, also consider *which* streets of value 
	- on a draw heavy board, bet earlier streets 
		- worse made hands are more likely to call, hoping you're on a draw
		- drawing hands are charged to see a turn/river
	- on a static board, you can afford to check the flop for deception

slowplaying
- don't slowplay a hand that should get 3 streets of value, since the third street of value is the most valuable
	- e.g. don't check back a set on the flop for deception or to let others catch up. goal is to stack someone that flopped top pair or two pair or a lower set
- slowplaying does not include checking a hand that has less than 3 streets of value, that's fine


[^1]: **Showdown equity:** chance your hand will win at showdown if rest of the board runs out. This is the percentage often displayed on poker videos
	
	**Folding equity:** the chance you get an opponent to fold when you run a successful bluff 
	
	**Equity-when-called:** Total equity your hand has after your raise is called. Includes the sum of your showdown equity and folding equity should you choose to bluff later streets


[^2]: large bets OR stack-committing bets:
	- large bet: a size you would only see once or twice an hour
	- stack-committing bet: you cannot imagine your opponent folding after making the bet 

[^3]: if you bet your hand on a given street and most of the time, worse hands will call, consider that a "street of value"

[^4]: top pair top kicker

[^5]: a board is dynamic if the best hand is likely to change after the turn and river
