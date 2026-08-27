# ECE-2112-PA1

Made by Iuryjane H. Pranada

This file contains the information regarding the Program Assignment 1 for the course "Advance Computer Programming" with the title code ECE2112. This assignment covers three python problems based on Module 1 - Base Computing with Python.

# A. Word Rotation Problem
Create a function named rotation_word() that accepts a non-empty string and moves its first character to the end while keeping the rest in order and preserving capitalization.

Code:
def rotate_word(text):
return text [1:] + text [0]

The first line of the code just defines the new function called rotate_word. Meanwhile, the second line returns the original string rotated by taking a slice from the second character to the end (text[1:]) and concatenating the first character (text[0]) onto the end.

Example:
rotate_word("python")

For example, passing "Python" evaluates text[1:] as "ython" and text[0] as "P", joining them into "ythonP" while keeping all original character capitalization intact.

# B. Username Builder Problem
Create a new function named make_username() that accepts two strings (a first and last name), converts all letters to lowercase, removes all spaces, and joins them with a period.

Code:
def make_username(first_name, last_name):
    final_first=first_name.lower().replace(" ", "")
    final_last=last_name.lower().replace(" ", "")
    return final_first + "." + final_last

This function creates a clean username by normalizing both inputs and joining them together. The first two lines convert first_name and last_name to lowercase using .lower() and strip out any spaces using .replace(" ", ""). The final line concatenates the cleaned first name, a period, and the cleaned last name.

Example:
make_username("Ada", "Lovelace")

For example, passing "Ada " and "Lovelace " transforms the inputs into "ada" and "lovelace", returning "ada.lovelace".

# Bookend Swap Problem
Create a new function named swap_bookends() that accepts a list of at least two elements. Unpack the list into first, middle, and last variables, then return a new list with the first and last elements swapped while keeping middle in its original order.

Code:
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]

This function swaps the first and last elements of a list using extended unpacking. Line 1 assigns the first item to first, the last to last, and all intermediate items to the list middle via the * operator. Line 2 returns a new list combining [last], middle, and [first].

Example:
swap_bookends([1, 2, 3, 4, 5, 6])

For example, swap_bookends([1, 2, 3, 4, 5, 6]) unpacks first=1, middle=[2, 3, 4, 5], and last=6, returning [6, 2, 3, 4, 5, 1].


