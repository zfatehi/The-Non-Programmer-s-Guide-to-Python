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

Now I’m going to move on to loops, which are exactly what they sound like; they perform a function over and over in a loop until the condition, which is specified, comes true. We’ll start with the `for` loop, using it to print our list:

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
You may be thinking, why is that so special? It’s just printing my list of movies, just not all in the same line. Trust me, I was thinking the same thing. 



