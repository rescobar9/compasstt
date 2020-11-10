# CompassTT

## Step 1

Select "Variables" on the left hand side menu and click on "Make a Variable"
Name your variable "Compass" (Do not include the "")

## Step 2
Select "Variables" on the left hand side menu again and drag the "set Compass to 0" inside the "Forever" block under "Calibrate compass"
```blocks
basic.forever(function () {
    Compass = 0
})
```
## Step 3
Select "Logic" on the left hand side menu and drag the "If-then else" block inside the "Forever" block under "Calibrate compass"

```blocks
basic.forever(function () {
    Compass = input.compassHeading()

    if (true) {
        
    } else if (true) {
        })
```

## Step 4
Select "Logic" on the left hand side menu and drag the "0 < 0" block an replace the "true" block.
Repeat the same step for "else if".

```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (0 < 0) {
    	
    } else if (0 < 0) {
    	
    }
})
```

## Step 5
Select "Variables" on the left hand side menu again and drag the "Compass" block and replace the first "0" in the "if" statement
Repeat the same steps for the "else if" statement.

```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 0) {
    	
    } else if (Compass < 0) {
    	
    }
})
```

## Step 6
Change the second "0" value after the "<" in the "if statement to 45
Repeat the same steps for the "else if" statement but changed the second "0" value after the "<" to 135.

```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 45) {
    	
    } else if (Compass < 135) {
    	
    }
})
```

## Step 7
Select "Basic" on the left hand side menu and drag the "show arrow North" block and place it under the "if" statement.
Select "Basic" on the left hand side menu again and drag the "show string "Hello!"" block and place it under the "show arrow North" block.
Replace the "Hello!" with an "N"
```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 45) {
    	basic.showArrow(ArrowNames.North)
         basic.showString("N")
    } else if (Compass < 135) {
    	
    }
})
```

## Step 8
Press the "+" sign below the "else if" statement then press the "+" sign below the "else" statement.
Press the "+" sign below the "else" statement again
```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 45) {
    	basic.showArrow(ArrowNames.North)
         basic.showString("N")
    } else if (Compass < 135) {
    	
    }else if (<  >) {
    	
    } else if (<  >) {
    	
    } else {
    	
    }
})
```



## Step 10
Right click on the "show arrow North" block on the first "if" statement and select "Duplicate"
Drag the duplicated copy to the next "else if" block and change the word "North" to "East".
Right click on the "show string N" block on the first "if" statement and select "Duplicate"
Drag the duplicated copy to the next "else if" block below the "show arrow east" block and change the letter "N" to "E".
Repeat the same steps for the next steps. Make sure you reflect what is shown on the code.

```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 45) {
    	basic.showArrow(ArrowNames.North)
         basic.showString("N")
    } else if (Compass < 135) {
    	basic.showArrow(ArrowNames.East)
         basic.showString("E")
    }else if (Compass < 225) {
    	basic.showArrow(ArrowNames.South)
         basic.showString("S")
    } else if (Compass < 315) {
    	basic.showArrow(ArrowNames.West)
         basic.showString("W")
    } else {
    	
    }
})
```

## Step 11
Right click on the "show arrow North" block on the first "if" statement and select "Duplicate"
Drag the duplicated copy to the last "else" block
Right click on the "show string "N"" block on the first "if" statement and select "Duplicate"
Drag the duplicated copy to the last "else" block below the "show arrow North" block.

```blocks
basic.forever(function () {
    Compass = input.compassHeading()
    if (Compass < 45) {
    	basic.showArrow(ArrowNames.North)
         basic.showString("N")
    } else if (Compass < 135) {
    	basic.showArrow(ArrowNames.East)
         basic.showString("E")
    }else if (Compass < 225) {
    	basic.showArrow(ArrowNames.South)
         basic.showString("S")
    } else if (Compass < 315) {
    	basic.showArrow(ArrowNames.West)
         basic.showString("W")
    } else {
    	basic.showArrow(ArrowNames.North)
         basic.showString("N")
    }
})
```

Congratulations, you did it!
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
