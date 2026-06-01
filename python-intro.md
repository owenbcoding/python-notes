# Program Structure

## Hello World

You are probably familiar with the phrase **"Hello World!"** if you've learned other programming languages in the past. This is a simple Python program named `greetings.py` that prints **"Hello World!"** to the output:

```python
def main():
    print('Hello World!')

if __name__ == '__main__':
    main()
```

## The `main()` Function

Curious why we used a `main` function to create the program? In Python, we frequently use the `main()` function to define the starting point of our program. Including `main()` allows us to import and run this program in another script.

Placing the `if` statement in our program checks whether the program is being run independently as the primary module or as a library in another script. If you run `greetings.py` on its own in the terminal, it will print **"Hello World!"**:

```bash
$ python greetings.py
Hello World!
```

## Comments

### What Are Comments?

In Python, comments are made with `#` to explain code at various points in the program. Comments are not executed as code and are used for documentation. There are two types of comments: **inline comments** and **block comments**.

### Inline Comments

Inline comments should be used when you have a short comment that you would like to include after a line of code.

```python
minutes = seconds / 60  # calculating minutes from seconds
```

### Block Comments

Block comments are used when you have multiple lines of comments that you'd like to include with your code. Unlike most languages that have special syntax for multiple-line comments, Python requires `#` on consecutive single lines.

```python
def calculate_minutes(seconds):
    # This function calculates the time in minutes
    # from the given seconds.
    minutes = seconds / 60
    return minutes
```