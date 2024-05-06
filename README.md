# CodeInPlace2024_Stanford_University-Projects

# [Project-1: Karel (Python Programming)- Archway Project](https://codeinplace.stanford.edu/cip4/share/uRDsiYVLeckoTvWA2Zaz)

* below is the karel python programming coding-

from karel.stanfordkarel import *

def main():
    """
    Karel starts facing East in the bottom left corner of the world and ends facing East in the bottom right corner of the world.
    """
    turn_left()
    move()
    move()
    move()
    turn_right()
    move()
    move()
    move()
    turn_right()
    move()
    move()
    move()
    turn_left()
    
def turn_right():
    turn_left()
    turn_left()
    turn_left()

if __name__ == '__main__':
    main()

![Screenshot (163)](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/1075d251-13a9-4d55-a2ba-1f3a125786e5)


# [Project-2: Karel (Python Programming)- Karel's Home Project](https://codeinplace.stanford.edu/cip4/share/Y24fSUOKbBfw14kevFB1)

* below is the karel python programming coding-

from karel.stanfordkarel import *

# File: shelter.py
# -----------------------------
# The warmup program defines a "main"
# function which should make Karel 
# move to the beeper, pick it up, and
# return home.
def main():
    move()
    move()
    turn_left()
    turn_left()
    turn_left()
    move()
    turn_left()
    move()
    pick_beeper()
    turn_left()
    move()
    move()
    turn_left()
    move()
    move()
    move()
    move()
    turn_left()
    move()
    move()
    move()
    move()
    turn_left()
    move()
    move()
    move()
    move()
    turn_left()
    move()
    move()
    turn_left()
    move()
    move()
    move()
    turn_left()
    turn_left()
    turn_left()
    move()
    turn_left()
    turn_left()
    turn_left()
def turn_right():
    turn_left()
    turn_left()
    turn_left()
    
if __name__ == '__main__':
    main()

![Screenshot (164)](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/ec74dbf1-bc06-436f-9727-f99bd85b2eec)


# [Project-3: Karel (Python Programming)- Stone Mason Karel Project](https://codeinplace.stanford.edu/cip4/share/h1HW9ZB6LnD6q5UFTLqd)

* below is the karel python programming coding-

from karel.stanfordkarel import *

"""
File: main.py
--------------------
When you finish writing this file, Karel should have repaired 
each of the columns in the temple
"""

def main():
    """
    You should write your code to make Karel do its task in
    this function. Make sure to delete the 'pass' line before
    starting to write your own code. You should also delete this
    comment and replace it with a better, more descriptive one.
    """
    for i in range(3):
        ascend_wall()
        move_to_wall()
        four_squares_apart()
    ascend_wall()
    move_to_wall()
    
   
def ascend_wall():
    turn_left()
    while front_is_clear():
        put_beeper()
        move()
    put_beeper()
    turn_around()
    

def move_to_wall():
    while front_is_clear():
        move()
    turn_left()

def four_squares_apart():
    for i in range(4):
        move()

def turn_right():
    for i in range(3):
        turn_left()

def turn_around():
    for i in range(2):
        turn_left()

if __name__ == '__main__':
    main()

![Screenshot (165)](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/9f6fdaec-b3ac-4400-8924-24e4fb0a75e4)

# [Project-4: Karel (Python Programming)- Fill Karel Project](https://codeinplace.stanford.edu/cip4/share/BUMsJkfmhW3NyoYZ1L83)

* below is the karel python programming coding-

from karel.stanfordkarel import *

"""
Karel should fill the whole world with beepers.
"""

def main():
    """
    You should write your code to make Karel do its task in
    this function. Make sure to delete the 'pass' line before
    starting to write your own code. You should also delete this
    comment and replace it with a better, more descriptive one.
    """
    while left_is_clear():
        fill_beepers()
        turn_back_row_position()
        move_to_wall()
        move_next_row()
    fill_beepers()

def fill_beepers():
    while front_is_clear():
        put_beeper()
        move()
    put_beeper()

def turn_back_row_position():
    while front_is_blocked():
        turn_around()

def move_next_row():
    while front_is_blocked():
        turn_right()
    move()
    turn_right()

def turn_around():
    for i in range(2):
        turn_left()

def move_to_wall():
    while front_is_clear():
        move()

def turn_right():
    for i in range(3):
        turn_left()

if __name__ == '__main__':
    main()

![Fill Karel](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/e032cb13-bbc0-43ff-a30c-5ffd3e2bcba2)



