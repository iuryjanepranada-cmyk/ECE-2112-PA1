# ECE-2112-PA1

Made by: Iuryjane H. Pranada, 2ECE-B

Made by Iuryjane H. Pranada

This file contains the information regarding the Program Assignment 1 for the course "Advance Computer Programming" with the title code ECE2112. This assignment covers three python problems based on Module 1 - Base Computing with Python.

# A. Word Rotation Problem
Create a new function named rotation_word() that accepts a non-empty string. It should also be able to move the first character to the end while keeping the rest in order and preserving capitalization.

Code:
def rotate_word(text):
    return text [1:] + text [0]

The first line of the code just defines the new function called rotate_word. Meanwhile, the second line returns the original string rotated by taking a slice from the second character to the end (text[1:]) and concatenating the first character (text[0]) onto the end.

Example:
rotate_word("python")

For example, passing "Python" evaluates text[1:] as "ython" and text[0] as "P", joining them into "ythonP" while keeping all original character capitalization intact.

# B. Username Builder Problem