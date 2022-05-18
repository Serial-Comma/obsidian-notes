# Pseudocode Syntax
### "because what's the point of making it simple?"

## Normal stuff

`DECLARE`
Syntax: `DECLARE <variable name> : <data type>`

What can you declare?

```C
INTEGER: 1,2,-3,0 //Basically Python int()
REAL: 4.7, 6.9, 3.141592654 //It's not float() because mr fong wants to make everyones life difficult
STRING: "This is a string", 'Single quotes arent strings because mr fong hates you'
BOOLEAN: TRUE, FALSE
DATE: 04/06/1989 (dd/mm/yyyy)
```

`CONSTANT`
Syntax: `CONSTANT <'variable' name> = <value>`
Constants don't exist in python,  thus making this very useful to our learning
```C
CONSTANT Mr_Fong = "Asshole"  //You do not have to declare a constant before you assign a value to it for some reason
CONSTANT My_Uni_L1R5 = 69
CONSTANT School_Budget = 0
```

## Operators
Addition : +
Subtraction: -
Multiplication: *
Division: / 
Greater Than: >
Less Than: <
Greater Than or Equal to: >=
Less Than or Equal to: <=
Equal to: =
Not Equal to: <>

AND
OR
NOT

## Input Output stuff

`OUTPUT, PRINT, PUT, DISPLAY` are all the same thing as far as you are concerned. For (somewhat) consistency with Python just use `PRINT` for everything to make your life easier
`WRITE` is your Python `file.write("Screw you")`

```C
DISPLAY "You Failed"
PRINT Results_Slip
PUT "Your Uni RP was"
OUTPUT 10
```

`READ` is your Python `file.read()`
`GET` is your Python `input("Why are you here")`
and for some reason A level pseudocode doesn't have `INPUT` even thought it kind of exists in O level computing and output literally has `OUTPUT`
```
READ Your_Mother
GET His_Virginity
```

## Loops
`WHILE-ENDWHILE` and `DOWHILE-ENDO` are the exact same thing ~~(even though while is supposed to be a precondition and dowhile is a postcondition irl???)~~ and are both precondition loops like your `while True:` in Python
```C
WHILE School_Budget <= 10:
	Spending_on_mantaining_existing_facilities <- 0
	Spending_on_new_campus <- Spending_on_new_campus + 1
	School_Budget <- School_Budget - 1
ENDWHILE
```

`REPEAT-UNTIL` has no equivalent in Python because Python has no post-condition loops (based) but just remember that whatever's in this loop always execute at least once, with the condition for repeat being asked for at the end of the loop
```C
REPEAT
	Repair_Classroom_Whiteboards <- FALSE
	JC_Dustbins <- JC_Dustbins - 1
	IP_Dustbins <- IP_Dustbins + 1
UNTIL JC_Dustbins == 0
```

`FOR` is your standard `for i in [1, x]:` loop in Python
```C
FOR Mental_Health <- 1 TO TJC_STUDENTS STEP 1
	
```