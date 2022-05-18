# Pseudocode Syntax
### "because what's the point of keeping it simple?"

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
CONSTANT School_Budget = 0 //Also apparently instead of using <- it uses = ??? What bs is this
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

These exist:
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

`FOR-ENDFOR` is your standard `for i in range(x):` loop in Python
```C
FOR count <- 1 TO TJC_STUDENT_MENTAL_HEALTH
	TJC_STUDENT_MENTAL_HEALTH[count] <- TJC_STUDENT_MENTAL_HEALTH[count] - 9000
ENDFOR
```

## Selection
`IF` does exactly what you think it does *if* it was consistent with Python
```C
IF No_of_lessons_with_no_breaks_in_a_row <= 10 //Take note there is no : at the end
	THEN
		No_of_lesson_with_no_breaks <- No_of_lessons_with_no_breaks + 999
	ELSE
		PRINT "Screw You"
ENDIF
```
you can also use `AND and OR` to smush multiple conditions together if you want to save time
```
IF Uni_RP <=60 AND Daddy = "RICH"
	THEN
		UNI_RP <- 90
ENDIF
```


`NOT` can be used in the case of `IF NOT TJC_STUDENT = "Straight"` but why would you do that when `IF TJC_STUDDENT <> "Stright"` exists and you save 5 characters


also make sure to use brackets if you have more than 3 conditions to keep it unambigious
```
IF (Students_Nearby <= 1 AND Teachers_Nearby <= 0) OR At_School == FALSE
	THEN
		Make_Love == TRUE
	ELSE
		Make_War == TRUE
ENDIF
```


## The only useful thing in pseudocode

`CASE-ENDCASE`
Syntax: 
```
CASE OF <variable_name>
	<value> : <do something>
	<value> : <do something>


	OTHERWISE <do something>
ENDCASE
```
This is probably the closest thing to Python dictionaries as you can get in pseudocode.
Its also a little more useful than dictionaries because it actually accepts ranges in its value which Python doesnt apparently
```
CASE OF possible_locations_in_school
	audi_with_people: PRINT "Hell no"
	audi_without_people: PRINT "If you're into it"
	LT1 : arousal <- arousal - 2000
	LT2 : arousal <- arousal + 2000
	physics_lab <- PRINT "Hell no"
	bio_lab <- PRINT "Hell yeah"

	OTHERWISE PRINT "Lets just do it in a love hotel"
ENDCASE
```

## Arrays
Unlike Python, Arrays in Pseudocode must always have a fixed and unchanging length which is declared at the start (Python is actually the exception because most programming languages have fixed length arrays too), so a `.append()` function for arrays doesn't exist

Anytime you're using an array and inputting values into it do something like this:
```C
CONSTANT ArrayLength = 20
DECLARE TJC_Student_Mental_Health : ARRAY[1:ArrayLength] OF INTEGER

FOR count <- 1 TO ArrayLength //You cant use range(len(TJC_Student_Mental_Health))
	PRINT "Input the mental health score of poor TJCian number" + count
	READ TJC_Student_Mental_Health[count]
ENDFOR
```
If youre really jazzed up and want to use arrays in a total of two (2) dimensions do this:
```C
DECLARE hot_singles_in_your_area : ARRAY [1:10,1:20] OF INTEGER
// This makes a matrix of 10 columns and 20 rows, yes its confusing 

FOR ROW <- 1 TO 20
	FOR ROW <- 1 TO 10
	PRINT "Input the value of row" + ROW + "and column" + COL
	READ hot_singles_in_your_area[ROW,COL]
ENDFOR
```
also the index of arrays in pseudocode start from 1 instead of 0. Why? Because fuck you, that's why.

## Functions

`PROCEDURE` is basically a more useless function because you cant return anything
Syntax:
`PROCEDURE name(x : INTEGER, y: STRING)`
Example:
```C
PROCEDURE Amount_of_hours_of_sleep(x : STRING)
	CASE OF x 
		GP_HW = TRUE: PRINT "10 Hours"
		Math_HW = TRUE : PRINT "9 Hours"
		Econs_HW = TRUE: PRINT "21 Hours"
		OTHERWISE PRINT "200 Hours"
ENDPROCEDURE

MAIN //You need this apparently

CALL Amout_of_hours_of_sleep("GP_HW")

ENDMAIN
```


`FUNCTION` is similar to Python's user-defined functions that you know and love, except a lot worse
Syntax: `FUNCTION name(x: REAL, y: INTEGER) RETURNS BOOL`
Example:
```C
FUNCTION amount_of_interest_i_have(x : STRING) RETURNS INTEGER
	CASE of X
		Econs = TRUE: RETURN 100
		Math = TRUE: RETURN 90
		Physics = True: RETURN 80
		GP = TRUE: RETURN 40
		Chinese = TRUE RETURN 0
	OTHERWISE RETURN 50
ENDFUNCTION

MAIN

CALL amount_of_interest_i_have("GP")

ENDMAIN
```
