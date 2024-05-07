# CodeInPlace2024_Stanford_University-Karel_Python_Projects

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

# [Project-5: Karel (Python Programming)-Warmup Karel Project](https://codeinplace.stanford.edu/cip4/share/rkb8AXL539ruRgPNsOZb)

* below is the karel python programming coding-

from karel.stanfordkarel import *

# File: warmup.py
# -----------------------------
# The warmup program defines a "main"
# function which currently just has one
# Command. Add two more commands to make karel: move(),
# pick_beeper(), move()
def main():
    move()
    pick_beeper()
    move()
   
if __name__ == '__main__':
    main()

![Warmup Karel-CIP2024](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/a99fc57a-eb64-466b-98fa-e58e79cd77af)

# [Project-6: Karel (Python Programming)-Piles Karel Project](https://codeinplace.stanford.edu/cip4/share/bRMM6VTtiSmcTN3IZA2k)

* below is the karel python programming coding-

  from karel.stanfordkarel import *

# File: piles.py
# -----------------------------
# The warmup program defines a "main"
# function which should make Karel
# pick up all the beepers in the world.
def main():
    move()
    # your code here
    while front_is_clear():
        pick_10_beeper()
        move()
        
        
def pick_10_beeper():
    for i in range(10):
        if beepers_present():
            pick_beeper()
    
           
# don't edit these next two lines
# they tell python to run your main function
if __name__ == '__main__':
    main()

![PILES KAREL](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/b0de7ae6-1712-4a41-be4f-8d9ab20af06e)

# [Project-7: Karel (Python Programming)-2024 Karel Project]

* below is the karel python programming coding-

from karel.stanfordkarel import *

"""
When you finish writing this file, Karel should be able to 
place 20 beepers, then 24 beepers, and end facing East to 
the right of the 24 beepers.
"""

def main():
    """
    You should write your code to make Karel do its task in
    this function. Make sure to delete the 'pass' line before
    starting to write your own code. You should also delete this
    comment and replace it with a better, more descriptive one.
    """
    if front_is_clear():
        put_20_beeper()
        move()
    
    if front_is_clear():
        put_24_beeper()
        move()
          
def put_20_beeper():
    for i in range(20):
        put_beeper()
        
def put_24_beeper():
    for i in range(24):
        put_beeper()
    
if __name__ == '__main__':
    main()

![Screenshot (166)](https://github.com/SHEETAL0812/codeinplace2024_stanford_university/assets/128026212/e0e4d7f0-71ec-40e8-86c2-da0f3cb7517c)




