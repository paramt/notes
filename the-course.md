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

#### Facing a raise 

TODO
### Blinds

TODO

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


- don't protect your hands 
	- value hands want to be called, bluffs want to generate folds
	- don't bet hands with little value hard like QT on Q97 to "protect it"
		- if you bet hard you've turned this hand into a bluff

### Bet sizing
- in general, big bets get folds and small bets get called. but people overestimate this effect
- typical players have a threshold of hand strength over which they call no matter what, and a threshold of hand strength under which they fold no matter what 
	- e.g. with trips on anything that's not 4-to-a-flush or 4-to-a-straight board - a particular player might call any bet
	- with king high on the river a particular player might fold to any bet 
- knowing these thresholds for other players is critical - you can never bluff them off a hand stronger than their strong threshold
- knowing their weak threshold is also useful - you can bluff them off with cheap bluffs (eg 15 into a pot of 100) profitably, because (enough of your opponent's hands fall below their calling threshold)[^6]

use bet sizing to extract maximum value from your good hands 

1. bet big enough with big hands so you can comfortably bet all in by the river. e.g. if you flop a set, goal is to win stacks => flop bet needs to be sizeable, don't slowplay by checking or betting small. you need to give yourself the chance to win stacks
2. sometimes you can squeeze in an extra street of value if you make your bet sizes smaller. e.g. you can turn TPMK[^7] hands into 3 streets of value by betting smaller. if you use the same strat as 1 (ie size such that you go all in by the river), then hands that call you will more often than not beat you. but with a smaller river size, you can still get called by worse. depends on the opponent
3. don't bet big with vulnerable hands. you want to invest more money in your stronger hands not your weaker hands, plus you want to take the winning hand to showdown
4. bet bigger than your opponents do
5. don't worry about tipping your hand strength with bet sizing (for now, will change with higher stakes)

### Multi-Way Pots and Loose Games
- if everyone calls light, don't be afraid to bet for value with even TPMK[^7]
- when you flop top pair, you bet. you keep betting (including river jam) unless someone raises you. when that happens, you fold (skill #2)
- 1 dimensional strategy, but works well at low stakes

### Final Thoughts 
> If you flop a hand with showdown value, the goal is to squeeze as much value from the hand as you can, then get it to showdown so you can realize its value. You can estimate a hand’s value by using our streets-of-value method. In your mind, create a plan for the hand. Determine how many times you can bet the hand and expect to be called by worse hands. Think about which turn cards will help you by adding streets of value, and which cards will hurt you and take value away. Think about which types of cards are more likely to fall.


re skill 2, on responding to large bets:

> The only time you consider calling is if you can think of a few hands you still beat that they might bet hard. That calling exception certainly comes up. But most of the calls I see at 1-2 involve hands that had no chance to win (unless the bettor was bluffing). You absolutely must learn to fold these hands without fail and without remorse.


## 1-2 Hand Quizzes

# Part III: Beating 2-5 Games

Part II skills were "playing your cards" skills. Part III skills focus on what opponents have rather than what we have. Mastering these skills should let you play a session or two completely blind, without losing too badly.

## Skill 4: Barreling
let's say you raise preflop and get called, heads up. on the flop opponent checks, you bet half pot. half the time opponent folds. other half of the time, he calls. on the turn, he checks and you bet half pot. half the time, he folds, other half of the time, he calls. on the river, he checks and you bet half pot. he folds half the time and calls the other half 

regardless of what your cards were, this would be a winning strategy 

how did the opponent misplay this? folds too often and doesn't raise 

a lot of players at 2-5 are at this level: they used to play too many hands, frequently lost money, and adapted by folding more hands (too many hands) 

most people are trusting large bets (including us: skill #2) and folding to them. we exploit this by barreling. this exploits the tendencies people have:
- they play too many hands preflop (so come into the flop with a wider range, missing most flops)
- they have a general trust of large bets

### Continuation Betting 
- cbet should not be about what you're representing, that's mostly irrelevant. rather, it's about what the opponent is holding
- e.g. we raise preflop with AQs, flop comes K42 rainbow. you don't cbet to "represent" the king, because people will fold not out of fear that the bettor hit a king, rather because they missed the flop 
- much more important to cbet on a flop like 842 rainbow than a flop like K42 rainbow
	- even if you can't represent hitting the flop, it's more likely the opponents missed
	-

### Barrelling Beyond The Flop
- opponents might call a flop bet with bottom pair or a gutshot, but they'll fold to a turn bet 
- opponents will put a value to their hand, and if the pot gets larger than the value they assigned to their hand, they'll fold (this can be fuzzy)
- we need to determine when opponents feel that their hand didn't make the cut
### Bet The Turn

> Above all, remember this about barreling: when they check to you on the turn, and you won’t be able to win a showdown without improvement, bet.

if you can't figure out when to bet, betting all your weak hands is better than betting none of them

bet large on the turn when it checks to you
- opponents play too many hands preflop, and make too many speculative calls on the flop 
- => they have way more hands by the turn than they should
- do this even if they have betting lead on the flop, as long as they check to you on the turn

- this is why you don't limp preflop
	- limping will make smaller pots, and smaller pots are less predictable

### Multiway Pots and Loose Games 
- don't barrel into 4 opponents with nothing, assume you'll get callers
- it's fine if you have a draw (even backdoors) as long as SPR[^8] is high, because the cbet  
	- builds the pot
	- keeps the nuts in your range, so you can steal the pot by representing it later (which is why high SPR matters) 
	- gives the opponent a chance to raise if they flopped big (so you can get out of the way)
		- opponents are less likely to slowplay in a multiway pot with draws out there

### Final Thoughts
- Skill 4 doesn't explain which hands to barrel with (that's Skill 5), but rather just says to barrel 
- test to determine if barrelling will be profitable in a game:
	- watch 20 hands. if more than half the hands play multiway, but <= 4 go to showdown (with someone having had to call a significant bet along the way), barrelling will be profitable

## Skill 5: Evaluating Board Texture 
- preflop is always the same, but once flop comes, hand rankings change 

### Static vs Dynamic Boards
Static: hand values (particularly at the top) are are relatively unlikely to change 

if you're ahead on the flop, you're likely ahead by the river

e.g. K73 rainbow 

Dynamic flop: hand values (particularly at the top) are likely to significantly change 

e.g. 974, two clubs

factors that make a board dynamic: 
1. low highest card
	1. overcards completely upset the ordering of the hands
2. flush and straight draws

importance of 2 is a bit overstated: an overcard changes the reordering of hands more drastically (since it's much easier to hit a pair than a flush)

example: 974 two clubs

we have A9

if a J comes, there's a total of 135 hands that hold a J and leapfrog us 
if a club comes, there's only 45 hands that have 2 clubs and leapfrog us


Barrelling 
- on a static board, you need fewer barrels to get the job done 
	- ie if your bluffs haven't worked on a static board after a flop and turn bet, you should probably give up 
	- but on a dynamic board, you might want to bluff the river as well, since your opponent could have missed draws or that your river bet means you outdrew them 

### Dry vs Wet Boards
Dry: few available draws 

K72 rainbow is dry, static

842 rainbow is dry, but dynamic



# My Thoughts 
a lot of the 1-2 skills too basic - I don't have much experience with live casino players, but this play would not hold up even in my 0.10/0.20 home games. here are some exploits 
- facing an open, most of the EP range is flatting. presumably because the risk of being squeezed is low in a low stakes game? I don't think I could flat in my 8 handed games as EP
- opponents definitely bluff way more often, always folding to a large river bet is too easily exploitable



[^1]: **Showdown equity:** chance your hand will win at showdown if rest of the board runs out. This is the percentage often displayed on poker videos
	
	**Folding equity:** the chance you get an opponent to fold when you run a successful bluff 
	
	**Equity-when-called:** Total equity your hand has after your raise is called. Includes the sum of your showdown equity and folding equity should you choose to bluff later streets


[^2]: large bets OR stack-committing bets:
	- large bet: a size you would only see once or twice an hour
	- stack-committing bet: you cannot imagine your opponent folding after making the bet 

[^3]: if you bet your hand on a given street and most of the time, worse hands will call, consider that a "street of value"

[^4]: top pair top kicker

[^5]: a board is dynamic if the best hand is likely to change after the turn and river

[^6]: (my note) example of playing ranges as opposed to particular hands

[^7]: top pair marginal kicker

[^8]: stack-to-pot ratio
