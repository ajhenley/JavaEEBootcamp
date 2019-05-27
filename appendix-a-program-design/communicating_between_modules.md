# Communicating Between Modules

At this point you've considered division of labor in your program. That's why you created modules. Now it's time to consider information flow.

Often you will need to send data to your modules as an input. You may then receive that data back as the output and all the processing steps would occur within the module.

You can accomplish this by passing parameters and returning values.

## Scope of a variable

The scope of a variable refers to the visibility of the variable. When is the variable available to your program or module? A variable declared inside a method or loop is available just to that method or loop; it does not exist elsewhere in your program.

Some programming languages allow you to declare global variables. Java is not one of those languages. This will save you endless heart-ache of your variable changing when you least expect it.

## Returning values

Modules \(when they represent functions\) can return values. When modules represent classes the class can contain methods that return values. A method can return a single value. That single value can be a class which would allow the method to return a complex value. But still a single value.

## Example: Converting miles/hour to kilometers/hour

```text
ConvertMph2Kmh
    prompt user "Enter miles/hour"
    get milesPerHour
    result = calculateKilometersPerHour(milesPerHour)
    display result
    END
calculateKilometersPerHour(milesPerHour)
    kph = milesPerHour * 0.62137119
    return kph
```

