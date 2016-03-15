# Lesson 1

First, we have to create a variable to work with, which you can think of as a box divided into numbered compartments with stuff inside that we can do things with (STUFF AND THINGS).

Here I am creating the variable movies, with a list of movies in it:

```
>>> movies = ["Life of Pi", "Monty Python and the Holy Grail", "Hitchhiker's Guide to the Galaxy"]
```

The print function lets me print anything I want, a variable, a string, or a string at a specific location, and it starts the numbering from 0:

```
>>> print (movies[1])
Monty Python and the Holy Grail
```

I can use another function, the length function len() to get the length of a string. 

```
>>> len(movies[0]+movies[2])
42
>>> len(movies[0])+len(movies[2])
42
```
(Before we go on, can we just talk about how the length of the "Life of Pi" and "Hitchhiker's Guide to the Galaxy" strings together is 42? Coincidence? I think not.)

Okay, back to it:
What is the difference between these two?
The first one creates a new string by combining the two in the positions 0 and 2 and takes the length, and the second one takes the length of both individually and adds them.
You get the same result.

The insert function allows me to insert a new string (item) at the specified location:

```
>>> movies.insert(2, "Lord of the Rings")
>>> print(movies)
['Life of Pi', 'Monty Python and the Holy Grail', 'Lord of the Rings', "Hitchhiker's Guide to the Galaxy"]
```

The remove function allows me to remove the first occurrence of the specified string (item) from wherever it is:

```
>>> movies.remove("Life of Pi")
>>> print(movies)
['Monty Python and the Holy Grail', 'Lord of the Rings', "Hitchhiker's Guide to the Galaxy"]
```

The pop function allows me to remove a string by specifying a location. If no location is specified, example: movies.pop() the last string is popped. 

```
>>> movies.pop(1)
'Lord of the Rings'
>>> print(movies)
['Monty Python and the Holy Grail', "Hitchhiker's Guide to the Galaxy"]
```

Another cool function is the append function; it allows me to do the same thing as:

```
>>> movies.insert(len(movies),"Nemo")
>>> print(movies)
['Monty Python and the Holy Grail', "Hitchhiker's Guide to the Galaxy", 'Nemo']
```
Which is basically letting me add a new string onto the end of my list.
See?

```
>>> movies.append("Nemo")
>>> print(movies)
['Monty Python and the Holy Grail', "Hitchhiker's Guide to the Galaxy", 'Nemo’]
```

Say you want to switch the positions of the last two strings on the lists:

```
>>> movies.append(movies.pop(1))
>>> print(movies)
['Monty Python and the Holy Grail', 'Nemo', "Hitchhiker's Guide to the Galaxy"]
```

There you go! Programmers being lazy!

But now say I don’t want to put that title at the end. I want to put it in the beginning!
Let’s try again:

```
>>> movies.insert(0, movies.pop(2))
>>> print(movies)
['Nemo', 'Monty Python and the Holy Grail', "Hitchhiker's Guide to the Galaxy"]
```

And we’ve done it! In a few deft keystrokes, we've ended up with a completely different list!



