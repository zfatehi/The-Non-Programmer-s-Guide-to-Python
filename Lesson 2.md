# Lesson 2

Now that we have a list of movies, it’s time to think about what we can do with it. Say we were running a movie database, or even simply publishing our favorite movies. What would be important information to include? I would like to see production years, but can you add numbers into a list containing strings? In other words, can you mix data types in a list in Python? Let’s find out:

```
>>> movies.insert(1, 1975)
>>> movies.insert(3, 2012)
>>> movies.insert(5, 2005)
>>> print(movies)
['Monty Python and the Holy Grail', 1975, 'Life of Pi', 2012, "Hitchhiker's Guide to the Galaxy", 2005]
```
Cool! (Or you can add the numbers to your list manually, which is a drag unless it is a short list like this).

Now I’m going to move on to loops, which are exactly what they sound like; they perform a function over and over in a loop until a certain point (I'll get into the specifics later, because it varies from loop to loop). We’ll start with the `for` loop, using it to print our list:

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
You can "translate" a `for` loop into English to make it easier to understand; for example, the `for` loop above would read:
"For the list movies, print each item until the list is over." In this `for` loop, I created the variable `each_item` and assigned it to hold each item in my movies list, one by one, so that every time one item in the list is printed, `each_item` gets reassigned to the next item in the list and that one gets printed. This happens again and again until the end of the list is reached.

You may be thinking, why is that so special? It’s just printing my list of movies, just not all in the same line. Trust me, I was thinking the same thing. Okay, so let's see what we can do with a `for` loop which includes a little function called `enumerate` which numbers the items in our list:

```
>>> for each_item, position in enumerate(movies):
	print (each_item, position)

0 Monty Python and the Holy Grail
1 1975
2 Life of Pi
3 2012
4 Hitchhiker's Guide to the Galaxy
5 2005
```
See what this gives me? My list, with position numbers built in so I can do things I learned earlier, like inserting or popping items; except I don't need to figure out their position numbers before I go ahead! Super convenient, and this is only an example of one of the cool things you can do with a `for` loop.



