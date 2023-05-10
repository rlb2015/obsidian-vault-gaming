# New-Game-Bennies
```
!Cbennies-reset -d "SWADE Bennies" -m Gronyon,Kayla|4,Voronwë
!Cbennies-reset -p "id" -d "SWADE Bennies" -q 3

```
# Bennies-showID
```
!bennies-show --ids
```
# Deal-New-Round
```
!deal-init
```
# Give-Bennie
```
!bennies-deal --deck "SWADE Bennies"  --quantity 1
```
# ReShuffle-and-Deal
```
!deal-init --reset
!deal-init
```
# Wild-Card-Roll
```
&{template:roll} {{name=WildCard Die Roll}} {{trait=?{myTrait}}} {{source=?{mySsource|Agility|Smarts|Spirit|Strength|Vigor}}} {{skill_rank=?{skill_die|d4|d6|d8|d10|d12}}}  {{skill_roll=[[?{skill_die}! - ?{Modifier|0}]] }} {{mook=[[1d0+1]]}} {{wild_die=[[1d6! - ?{Modifier|0}]]}} 
```
# table-allied-personalities
```
/w gm  &{template:info} {{name=Allied Personalities Table}} {{Result=[[1t[Allied-Personalities]]] }}
```
# table-dynamic-backlash
```
&{template:info} {{name=Dynamic Backlash Table}} {{Result=[[1t[Dynamic-Backlash]]] }}
```
# table-injury
```
&{template:info} {{name=Injury Table}} {{Result=[[1t[Injury]]] }}
```
# table-reaction
```
/w gm &{template:info} {{name=Reaction Table}} {{Result=[[1t[Reaction]]] }}
```
# table-vehicle-critical-hits
```
&{template:info} {{name=Vehicle Critical Hits Table}} {{Result=[[1t[Vehicle-critical-hits]]] }}
```
# table-vehicle-out-of-controler
```
&{template:info} {{name=Vehicle Out of Control Table}} {{Result=[[1t[Vehicle-out-of-control]]] }} {{Note=Damage caused by an Out of Control roll doesn’t trigger another Out of Control roll, but a Wound triggers a Critical Hit as usual.}} 
```
# Mook-Roll
```
&{template:roll} {{name=WildCard Die Roll}} {{trait=?{myTrait}}} {{source=?{mySsource|Agility|Smarts|Spirit|Strength|Vigor}}} {{skill_rank=?{skill_die|d4|d6|d8|d10|d12}}}  {{skill_roll=[[?{skill_die}! - ?{Modifier|0}]] }} {{mook=[[1d0]]}} {{wild_die=[[1d6! - ?{Modifier|0}]]}} 
```
# Raise-Calculator
```
/em Calculated this many raises: [[floor({?{Number|1} - ?{Target|4}}/4)]]
```
# 