# NumPy

NumPy is a Python package to efficiently do data science. Learn to work with the NumPy array, a faster and more powerful alternative to the list, and take your first steps in data exploration.

## Your First NumPy Array

In this chapter, we're going to dive into the world of baseball. Along the way, you'll get comfortable with the basics of `numpy`, a powerful package to do data science.

A list `baseball` has already been defined in the Python script, representing the height of some baseball players in centimeters. Can you add some code here and there to create a `numpy` array from it?

### Instructions - First NumPy Array

- Import the `numpy` package as `np`, so that you can refer to `numpy` with `np`.
- Use [np.array()](http://docs.scipy.org/doc/numpy-1.10.0/glossary.html#term-array) to create a `numpy` array from `baseball`. Name this array `np_baseball`.
- Print out the type of `np_baseball` to check that you got it right.

## Baseball players' height

You are a huge baseball fan. You decide to call the MLB (Major League Baseball) and ask around for some more statistics on the `height` of the main players. They pass along data on more than a thousand players, which is stored as a regular Python list: height. The height is expressed in inches. Can you make a `numpy` array out of it and convert the units to meters?

`height` is already available and the `numpy` package is loaded, so you can start straight away (Source: [stat.ucla.edu](http://wiki.stat.ucla.edu/socr/index.php/SOCR_Data_MLB_HeightsWeights)).

### Instructions - Baseball players height

- Create a `numpy` array from `height`. Name this new array `np_height`.
- Print `np_height`.
- Multiply `np_height` with `0.0254` to convert all height measurements from inches to meters. Store the new values in a new array, `np_height_m`.
- Print out `np_height_m` and check if the output makes sense.

## Baseball player's BMI

The MLB also offers to let you analyze their weight data. Again, both are available as regular Python lists: `height` and `weight`. `height` is in inches and `weight` is in pounds.

It's now possible to calculate the BMI of each baseball player. Python code to convert `height` to a `numpy` array with the correct units is already available in the workspace. Follow the instructions step by step and finish the game!

### Instructions - Baseball player's BMI

- Create a `numpy` array from the `weight` list with the correct units. Multiply by `0.453592` to go from pounds to kilograms. Store the resulting `numpy` array as `np_weight_kg`.
- Use `np_height_m` and `np_weight_kg` to calculate the BMI of each player. Use the following equation:

BMI=weight(kg)height(m)2

Save the resulting numpy array as bmi.

- Print out bmi.
