# Lesson 3

Now that I've generally gone through how a `for` loop, I can take a look at other loops and how they work. A `while` loop, which can take the place of a `for` loop, is much more specific than a while loop but can be made to the same thing.

From the last lesson, we created the `for` loop below to print out our list of movies:

```
>>> for each_item in movies:
    print(each_item)

Monty Python and the Holy Grail
1975
Life of Pi
2012
Hitchhiker's Guide to the Galaxy
2005
```

Now, we can create a `while` loop to do the same thing as this `for` loop above:
```
>>> count = 0
>>> while count < len(movies):
	print(movies[count])
	count = count+1

	
Monty Python and the Holy Grail
1975
Life of Pi
2012
Hitchhiker's Guide to the Galaxy
2005
```
This while loop is saying something a little different than our previous `for` loop; It says that "While the position count has not reached the end of the list, or the last postion in the variable 'box' we've called movies, keep printing the items in the list." In this loop, I have to define the count before the loop. Another important thing to note is like in the `for` loop, everytime an iteration (or repitition) of the loop is run, the variable `count` that I created is reassigned to the next position in the list (which is why we have set `count = count+1` for each iteration).

So, all it's doing is the same thing our `for` loop did from before, it's way more complicated, with way more room for error. So why use it at all? Seems pointless. However, after some research, 
