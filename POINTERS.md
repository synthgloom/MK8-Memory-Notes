# Pointer notes for Mario Kart 8

#### This file contains information about certain Pointers and where they lead to.

## _In-Game Data_
|  Pointer Notation            | Address it points to    |          Notes
|------------------------------|-------------------------|----------------------
|[[0x3FBA92BC] + 0x20] + 0x13C |Anti-gravity kart glow   |00000000 = Glowing, 3F800000 = Not Glowing
|[[0x3FBA92BC] + 0x20] + 0x140 |Anti-gravity kart glow radius|3F800000 = Normal?
|[[0x3FBA92BC] + 0x20] + 0x145 |Kart/Player Effects      |*See Below
|[[0x3FBA92BC] + 0x20] + 0x148 |Timer of some sort       |None
|[[0x3FBA92BC] + 0x20] + 0x14C |Player has moved from start?|00000000 = False, 3F800000 = True
|[[0x3FBA92BC] + 0x20] + 0x154 |Anti-gravity kart        |00000000 = Off, 3F800000 = On
|[[0x3FBA92BC] + 0x20] + 0x158 |Race has started?        |Decimal Value. 1 = True, 0 = False
|[[0x3FBA92BC] + 0x20] + 0x15C |Countdown speed buildup  |3F800000 = will explode, 3F7D2F1B = max buildup
|[[0x3FBA92BC] + 0x20] + 0x160 |Star power timer         |Decimal Value
|[[0x3FBA92BC] + 0x20] + 0x190 |Kart crushed state timer |Decimal Value
|[[0x3FBA92BC] + 0x20] + 0x75  |Countdown State          |01000000 = Can't move, 01010000 = Can move
|[[0x3FBA92BC] + 0x20] + 0x9C  |Kart Size X              |3F800000 = Normal
|[[0x3FBA92BC] + 0x20] + 0xA0  |Kart Size Y              |3F800000 = Normal
|[[0x3FBA92BC] + 0x20] + 0xA4  |Kart Size Z              |3F800000 = Normal
|[[0x3FBA92BC] + 0x20] + 0xA8  |Kart Overall Size        |3F800000 = Normal
|[[0x3FBA92BC] + 0x20] + 0xFC  |Control State?           |*Decimal Value
|[[0x3FBA92BC] + 0x20] + 0x5320|handling1                |Float Value
|[[0x3FBA92BC] + 0x20] + 0x5324|handling2                |Float Value
|[[0x3FBA92BC] + 0x20] + 0x5328|handling3                |Float Value
|[[0x3FBA92BC] + 0x20] + 0x53AC|Kart Max Speed           |Float Value
|[[0x3FBA92BC] + 0x20] + 0x53BC|Kart Boost Speed         |Float Value
|[[0x3FBA92BC] + 0x20] + 0x52E4|Kart Current Speed       |Float Value
|[[0x3FBA92BC] + 0x20] + 0x505C|Gravity Strength         |3F800000 = Normal Gravity
|[[0x3FBA92BC] + 0x20] + 0x5544|Drift Direction          |Decimal Value. 4 = Left, 5 = Right
|[[0x3FBA92BC] + 0x20] + 0x555C|Blue Drift Buildup Timer?|Float Value
|[[0x3FBA92BC] + 0x20] + 0x557C|Turn Direction           |Float value. Negative = Right, Positive = Left
|[[0x3FBA92BC] + 0x20] + 0x55A4|Drift Time Counter       |Float Value. 300 = Blue, 600 = Orange
|[[0x3FBA92BC] + 0x20] + 0x55A8|Drift State              |Decimal Value. 1 = Blue, 2 = Orange
|[[0x3FBA92BC] + 0x20] + 0x55AC|Drift Time Counter 2     |Decimal Value. 55 = Blue, 150 = Orange
|[0x3FB3CD70] + 0x50           |Amount of circling items |Determines how many items circle around you. Offline only.
|[0x3FB3CD70] + 0x54           |Amount of circling items2|Determines how many circling items you have left/can use. Offline only.
|[0x3FB3CD70] + 0x12C          |Displayed Item From Block|*000000XX = Item in player's hand. Offline only.
|[0x3FB3CD70] + 0x130          |Last Item From Block     |*000000XX = Last Item player got. Offline only.
|[0x3FB3CD70] + 0x134          |Actual Item From Block   |*000000XX = Actual Item player gets. Offline only.
|[0x3FB3CD70] + 0x140          |Item Block Rotation Speed|FFFFFFFF = Slow/No Rotation. Offline only.
|[0x3FB3CD70] + 0x84           |Time since last item use |Decimal Value. Offline only.

*See [here](https://github.com/Megabyte918/MK8-Cheat-Codes/blob/master/Kart%20Effect%20Modifier) for more information about effects. Values are shifted to the right by 2 bytes. So for example the effect of 00001000 would display as 00000010 in memory.

*0 = Not moving, 1 = Forward, 2 = Backward, 8 = Hop/Drift, 512 = Using Item, 1024 = Looking behind.
 Combos can be calculated just like they can with button activators.
 
 *See [here](https://github.com/Megabyte918/MK8-Cheat-Codes/blob/master/Item%20Hack) for more information on Item ID's