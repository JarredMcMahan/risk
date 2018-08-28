# risk



Support up to 6 players
	- N={2,3,4,5,6}

Prompt players for 3 actions
	1. Getting and placing new units based on territory owned (Ask where to put units, display owned territories)
2. Attacking (Yes or no)
3. Fortifying your position (Move units?)
	
World set up
	- 42 territories in 6 continents
	- Territories are split between each player by random draw of territory cards
		- If player count is >2 each get 40-((N-2)*5) Infantry unit
		- If players = 2 then each player gets 40 units
			- Should ask where to put pieces?
				1. Alaska
				2. Alberta
				etc..

Units
	- Infantry = 1 Infantry unit
	- Cavalry = 5 Infantry units
	- Artillery = 10 Infantry Units or 2 Cavalry

Cards
	- 42 cards with a territory and a picture of a unit plus 2 wild
		- Probably easier to randomize within range of units and Territories
		- max of 2 wild cards

Turn
1. New Units
	- Units each turn are granted based on:
		- Number of territories
			- Number of territories / 3
			- Minimum of 3 if territories are less than 9
		- Value of whole continents you control
			1. Asia = 7
			2. North America = 5
			3. Europe = 5
			4. Africa = 3
			5. South America = 2
			6. Australia = 2
		- Value of cards traded in (3 cards)
			- 3 cards with the same unit
			- One of each unit
			- 2 plus a wild card
		- Value of specific territory pictured on card
	           - If you own a territory in the card you get an extra 2 units (max 2)
	
2. Attacking
	- A player does not have to attack
	- Can only attack territory adjacent
		- Is the a more practical way than dozens of lists/arrays?
	- Must have 2+ units on a territory
	- If choosing to attack a territory, you can attack another adjacent territory at the same time.
	- Assign button press to end turn (better than a dozen popups eery attack)
	- if attacking, Roll dice with opponent (Must have at least one more unit in territory than the number of dice. i = units, i>number of dice. Max 3 dice.
	- Cannot attack with only one unit because if i=1 then dice!=1
- if defending, roll 1 or 2 dice, dice is the willing number of units the defender is willing to lose. 
	
Dice:
	- if attack > defender, defender loses units = dice rolled
	- if defender > attacker, attacker loses units = dice rolled
		- if defender = attacker, attacker loses one unit

3. Fortifying
	- Units may be moved across any adjacent territories
	- Must leave behind at least one unit.

Trade in sets (set increases by 1 per turn in)
	- Set 1: 3 units
	- Set 2: 5 units
	- Set 3: 8 unites
	- Set 4: 10 unites
	- Set 5: 12 unites
	- Set 6: 15 unites
	- Set >6: 15+(5*(N-6))

Win = 1 player owns all territory
lose = player has no territory

