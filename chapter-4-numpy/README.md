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

## Lightweight baseball players

To subset both regular Python lists and `numpy` arrays, you can use square brackets:

```py
x = [4 , 9 , 6, 3, 1]
x[1]
import numpy as np
y = np.array(x)
y[1]
```

For `numpy` specifically, you can also use boolean `numpy` arrays:

```py
high = y > 5
y[high]
```

The code that calculates the BMI of all baseball players is already included. Follow the instructions and reveal interesting things from the data!

### Instructions - Lightweight baseball players

- Create a boolean `numpy` array: the element of the array should be `True` if the corresponding baseball player's BMI is below 21. You can use the `<` operator for this. Name the array `light`.
- Print the array `light`.
- Print out a `numpy` array with the BMIs of all baseball players whose BMI is below 21. Use `light` inside square brackets to do a selection on the `bmi` array.

## NumPy Side Effects

As Filip explained before, `numpy` is great for doing vector arithmetic. If you compare its functionality with regular Python lists, however, some things have changed.

First of all, `numpy` arrays cannot contain elements with different types. If you try to build such a list, some of the elements' types are changed to end up with a homogeneous list. This is known as type coercion.

Second, the typical arithmetic operators, such as `+`, `-`, `*` and `/` have a different meaning for regular Python lists and `numpy` arrays.

Have a look at this line of code:

```py
np.array([True, 1, 2]) + np.array([3, 4, False])
```

Can you tell which code chunk builds the exact same Python object? The `numpy` package is already imported as `np`, so you can start experimenting in the IPython Shell straight away!

- [ ] np.array([True, 1, 2, 3, 4, False])
- [x] np.array([4, 3, 0]) + np.array([0, 2, 2])
- [ ] np.array([1, 1, 2]) + np.array([3, 4, -1])
- [ ] np.array([0, 1, 2, 3, 4, 5])

## Subsetting NumPy Arrays

You've seen it with your own eyes: Python lists and `numpy` arrays sometimes behave differently. Luckily, there are still certainties in this world. For example, subsetting (using the square bracket notation on lists or arrays) works exactly the same. To see this for yourself, try the following lines of code in the IPython Shell:

```py
x = ["a", "b", "c"]
x[1]

np_x = np.array(x)
np_x[1]
```

The script on the right already contains code that imports `numpy` as `np`, and stores both the height and weight of the MLB players as `numpy` arrays.

### Instructions - Subsetting NumPy Arrays

- Subset `np_weight` by printing out the element at index 50.
- Print out a sub-array of `np_height` that contains the elements at index 100 up to **and including** index 110.

## Your First 2D NumPy Array

Before working on the actual MLB data, let's try to create a 2D `numpy` array from a small list of lists.

In this exercise, `baseball` is a list of lists. The main list contains 4 elements. Each of these elements is a list containing the height and the weight of 4 baseball players, in this order. `baseball` is already coded for you in the script.

### Instructions - Your First 2D NumPy Array

- Use [np.array()](http://docs.scipy.org/doc/numpy-1.10.0/glossary.html#term-array) to create a 2D `numpy` array from `baseball`. Name it `np_baseball`.
- Print out the type of `np_baseball`.
- Print out the `shape` attribute of `np_baseball`. Use `np_baseball.shape`.

## Baseball data in 2D form

You have another look at the MLB data and realize that it makes more sense to restructure all this information in a 2D `numpy` array. This array should have 1015 rows, corresponding to the 1015 baseball players you have information on, and 2 columns (for height and weight).

The MLB was, again, very helpful and passed you the data in a different structure, a Python list of lists. In this list of lists, each sublist represents the height and weight of a single baseball player. The name of this embedded list is `baseball`.

Can you store the data as a 2D array to unlock `numpy`'s extra functionality?

### Instructions - Baseball data in 2D form

- Use [np.array()](http://docs.scipy.org/doc/numpy-1.10.0/glossary.html#term-array) to create a 2D `numpy` array from `baseball`. Name it `np_baseball`.
- Print out the `shape` attribute of `np_baseball`.

