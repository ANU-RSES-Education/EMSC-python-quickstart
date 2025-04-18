---
title: Python on the web
author:
    - Louis Moresi
    - Andrew Valentine
format:
  html:
    code-links: false
kernelspec:
  name: python3
  display_name: 'Python 3'
---

:::{note}
# Summary

In this section we'll discover how to run a basic python script (in the web browser) and what to expect in terms of editing, reloading, printing output and saving our work.
:::

There are many different ways to run python code. For the simplest tasks, a web browser is all you need to edit and run simple tasks. In this introductory session, we will use a python interpreter embedded in each web page to learn the basic language itself.

You will find examples of python code such as this one which contains some Python code which you can copy but which you can't run and you can't edit. Note that the code is highlighted (coloured) by meaning.

```{code-cell} python
# A simple script (with a descriptive comment)
print("Welcome to python !")
```

We use these blocks to give you examples and fragments of code that you can use later. Other code blocks have a `run` button and they can usually be edited (and, don't worry, they can be reset if you make a mistake). We use these **live** code blocks for you to try things out. Give it a go (you can't break anything).

```{code-cell} python
# A simple script (with a descriptive comment)
print("Welcome to python !")
```

Generally, we'll use the live code blocks as part of an exercise for you to try something specific. The exercise blocks look like this:

:::{tip}
:class: dropdown

## Exercise 1 - Run a script / edit a script

 The code box in this exercise **is** editable. If you click in this box, and then press <kbd>Shift</kbd>+<kbd>⏎</kbd> (i.e. hold down the <kbd>Shift</kbd> key on your keyboard and then hit the return key) the code will be run, and any output is displayed underneath. You can also use the run button if you prefer.

```{code-cell} python
# Blank code cell (this line is a comment)
print("Welcome to python !")
```

Note there is a clipboard button to copy your answer and this is quite important because it is not saved anywhere. If you want to keep answers to your exercises, have a separate notebook / editor handy.

When you have finished, you can collapse this exercise:

![](Images/CollapseThisExercise.png){.lightbox width=50% fig-align=center}
:::

Usually we will collapse the exercises by default and you'll need to open them to access the instructions and the code.
We can start right now ...

::: {tip}
:class: dropdown

## Exercise 2 - Calculations

We've already seen a couple of examples of Python code. Now let's try making something from scratch. One thing we can do is simply use Python like a calculator!

Try typing simple arithmetic into the code cell below and see what happens. For example, try entering

```{code-cell} python
3+17
```

```{code-cell} python
# Blank


```

You can also use the operators `*`, `-`, `/` (for division), and the parentheses `()`. Finally, `**` is used to raise a number to some power, so that $3^2$ is entered as `3**2`. Keep trying new calculations !

**What happens if you enter two lines of calculations and run ?** For example:

```{code-cell} python
3+17
5*9
```
Can you think how to get both of the answers to (hint) print out ?

:::


### Comments

In the examples above, you may have noticed the line

```{code-cell} python
# A simple script (with a descriptive comment)

```

which doesn't look as though it ought to be valid Python code. This is a 'comment' line: the computer ignores the `#` and anything following it on the same line. Comments should be used to document information that helps people to understand how the code works internally. This may seem like a waste of time - but you (or your colleagues) will be grateful in two years' time when you find you need to change something! The comment character can also be useful for 'switching off' lines of code without deleting them. For example, look at this piece of code:

```{code-cell} python
def readDataFile(fp):
    # This function assumes that fp is
    # a valid file-like object and that the
    # file has already been opened for reading
    header = fp.readline()
    # print(header)
    [...]
```

The first three lines of comments provide information recording some of the assumptions the programmer made when writing this function (don't worry if it doesn't make sense yet!). The fourth comment line is a piece of code that has been 'commented out': we don't want to routinely print the file header, but it is useful to be able to reinstate this easily in case we encounter problems and need to check what the function has read.

In fact, 'commenting out' code is so common that most editors provide a straightforward way to do it. If you select a block of code and press <kbd>Ctrl</kbd>+<kbd>/</kbd> (or on a Mac, <kbd>⌘</kbd>+<kbd>/</kbd>), the selected lines will all be changed to begin with `#` comment characters. Pressing <kbd>Ctrl</kbd>+<kbd>/</kbd> again will restore the original version. Smart editors know how to do this for many different languages.



### Sandbox

::: {warning}
:class: dropdown

## Coding scratch space


```{code-cell} python
## Scratch space / notepad

print("Comment out this code with the keyboard shortcut !")


```
:::
