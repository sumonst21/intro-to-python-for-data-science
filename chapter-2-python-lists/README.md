# Python Lists
Learn to store, access and manipulate data in lists: the first step towards efficiently working with huge amounts of data.


## Create a list
As opposed to int, bool etc., a list is a compound data type; you can group values together:

```

a = "is"
b = "nice"
my_list = ["my", "list", a, b]

```

After measuring the height of your family, you decide to collect some information on the house you're living in. The areas of the different parts of your house are stored in separate variables for now, as shown in the script.

 - Create a list, areas, that contains the area of the hallway (hall), kitchen (kit), living room (liv), bedroom (bed) and bathroom (bath), in this order. Use the predefined variables.

- Print areas with the `print()` function.

## Create list with different types
A list can contain any Python type. Although it's not really common, a list can also contain a mix of Python types including strings, floats, booleans, etc.

The printout of the previous exercise wasn't really satisfying. It's just a list of numbers representing the areas, but you can't tell which area corresponds to which part of your house.

The code on the right is the start of a solution. For some of the areas, the name of the corresponding room is already placed in front. Pay attention here! "bathroom" is a string, while bath is a variable that represents the float 9.50 you specified earlier.


## Select the valid list

A list can contain any Python type. But a list itself is also a Python type. That means that a list can also contain a list! Python is getting funkier by the minute, but fear not, just remember the list syntax:
```
my_list = [el1, el2, el3]
```
Can you tell which ones of the following lines of Python code are valid ways to build a list?
```
A. [1, 3, 4, 2] B. [[1, 2, 3], [4, 5, 7]] C. [1 + 2, "a" * 5, 3]
```

## List of lists
As a data scientist, you'll often be dealing with a lot of data, and it will make sense to group some of this data.

Instead of creating a flat list containing strings and floats, representing the names and areas of the rooms in your house, you can create a list of lists. The script on the right can already give you an idea.

Don't get confused here: "hallway" is a string, while hall is a variable that represents the float 11.25 you specified earlier.

## Subset and conquer
Subsetting Python lists is a piece of cake. Take the code sample below, which creates a list x and then selects "b" from it. Remember that this is the second element, so it has index 1. You can also use negative indexing.
```
x = ["a", "b", "c", "d"]
x[1]
x[-3] # same result!
```
Remember the areas list from before, containing both strings and floats? Its definition is already in the script. Can you add the correct code to do some Python subsetting?

 > example code for Subset and conquer added on the script.py

## Subset and calculate
After you've extracted values from a list, you can use them to perform additional calculations. Take this example, where the second and fourth element of a list x are extracted. The strings that result are pasted together using the + operator:
```
x = ["a", "b", "c", "d"]
print(x[1] + x[3])
```
 > example code for Subset and calculate  added on the script.py

## Slicing and dicing
Selecting single values from a list is just one part of the story. It's also possible to slice your list, which means selecting multiple elements from your list. Use the following syntax:

 > my_list[start:end]

The start index will be included, while the end index is not.

The code sample below shows an example. A list with "b" and "c", corresponding to indexes 1 and 2, are selected from a list x:

```
x = ["a", "b", "c", "d"]
x[1:3]
```

The elements with index 1 and 2 are included, while the element with index 3 is not.


## Subsetting lists of lists
You saw before that a Python list can contain practically anything; even other lists! To subset lists of lists, you can use the same technique as before: square brackets. Try out the commands in the following code sample in the IPython Shell:
```
x = [["a", "b", "c"],
     ["d", "e", "f"],
     ["g", "h", "i"]]
x[2][0]
x[2][:2]
```
x[2] results in a list, that you can subset again by adding additional square brackets.

What will house[-1][1] return? house, the list of lists that you created before, is already defined for you in the workspace. You can experiment with it in the IPython Shell.

## List Manipulation 
###### 
## Replace list elements
Replacing list elements is pretty easy. Simply subset the list and assign new values to the subset. You can select single elements or you can change entire list slices at once.

Use the IPython Shell to experiment with the commands below. Can you tell what's happening and why?
```
x = ["a", "b", "c", "d"]
x[1] = "r"
x[2:] = ["s", "t"]
```
For this and the following exercises, you'll continue working on the areas list that contains the names and areas of different rooms in a house.

## Extend a list
If you can change elements in a list, you sure want to be able to add elements to it, right? You can use the + operator:
```
x = ["a", "b", "c", "d"]
y = x + ["e", "f"]
```

You just won the lottery, awesome! You decide to build a poolhouse and a garage. Can you add the information to the areas list?
 > example code added on the script.py

## Delete list elements
Finally, you can also remove elements from your list. You can do this with the del statement:
```
x = ["a", "b", "c", "d"]
del(x[1])
```

Pay attention here: as soon as you remove an element from a list, the indexes of the elements that come after the deleted element all change!

The updated and extended version of **areas** that you've built in the previous exercises is coded below. You can copy and paste this into the IPython Shell to play around with the result.
```
areas = ["hallway", 11.25, "kitchen", 18.0,
        "chill zone", 20.0, "bedroom", 10.75,
         "bathroom", 10.50, "poolhouse", 24.5,
         "garage", 15.45]
```
There was a mistake! The amount you won with the lottery is not that big after all and it looks like the poolhouse isn't going to happen. You decide to remove the corresponding string and float from the **areas** list.

The ** ;** sign is used to place commands on the same line. The following two code chunks are equivalent:
```
# Same line
command1; command2

# Separate lines
command1
command2
```

Which of the code chunks will do the job for us?

###### Possible Answers
- [ ] del(areas[10]); del(areas[11])
- [ ] del(areas[10:11])
- [x] del(areas[-4:-2])
- [ ] del(areas[-3]); del(areas[-4])

## Inner workings of lists
At the end of the video, Filip explained how Python lists work behind the scenes. In this exercise you'll get some hands-on experience with this.

The Python code in the script already creates a list with the name **areas** and a copy named **areas_copy**. Next, the first element in the **areas_copy** list is changed and the **areas** list is printed out. If you hit Run Code you'll see that, although you've changed **areas_copy**, the change also takes effect in the **areas** list. That's because areas and **areas_copy** point to the same list.

If you want to prevent changes in **areas_copy** from also taking effect in **areas**, you'll have to do a more explicit copy of the **areas** list. You can do this with [list()](https://docs.python.org/3/library/functions.html#func-list) or by using `[:]`.
 > example code added to script.py