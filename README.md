# UNITTEST library
Python provides us with a batteries-included test module that is part of the Python standard library.
This testing framework is called **Unittest**.

## How to create a test:
1. Create two (2) files:    
    (1) where we will build our function (eg, evens.py)     
    (2) where we will write our tests (eg, test_evens.py)     
(Unittest requires that our **test filename** starts with the word ‘**test**’,  
followed by an underscore and a descriptive name of what we’re testing.)

2. Import the Unittest module into our test file.
    * Simply type import Unittest.  
    (Unittest is part of Python’s  standard library, so we don’t need to install it.)

3. Create a test case (eg, create `class TestEvens(unittest.TestCase)`)  
(Our class needs to inherit from the unittest.TestCase class)   
    * For now, pass in the statement `pass`         

4. Add `unittest.main()`.

5. On the 2nd file (eg, evens.py), create a function (eg, `def even_number_of_evens(numbers): return None`)     
    (A) Add your list of test ideas to our function as **docstring**.    
    (so we can refer to that if we need a reminder of what we could be testing for)

6. Import the function into the test file.

7. In the TEST FILE (eg, test_evens.py), write a test (tests whether our function returns True)     
    * This method should start with the word ‘**test**’. (If not, it will be ignored and won't run when we run the test file.)    
    * Pass in the **self** keyword.
    * Create either a single assert or many asserts (eg, `self.assertTrue()`)

8. Run the code using the command `python3 test_evens.py`


## Gitpod Reminders

To run a frontend (HTML, CSS, Javascript only) application in Gitpod, in the terminal, type:

`python3 -m http.server`

A blue button should appear to click: _Make Public_,

Another blue button should appear to click: _Open Browser_.

To run a backend Python file, type `python3 app.py`, if your Python file is named `app.py` of course.

A blue button should appear to click: _Make Public_,

Another blue button should appear to click: _Open Browser_.

In Gitpod you have superuser security privileges by default. Therefore you do not need to use the `sudo` (superuser do) command in the bash terminal in any of the lessons.

To log into the Heroku toolbelt CLI:

1. Log in to your Heroku account and go to *Account Settings* in the menu under your avatar.
2. Scroll down to the *API Key* and click *Reveal*
3. Copy the key
4. In Gitpod, from the terminal, run `heroku_config`
5. Paste in your API key when asked

You can now use the `heroku` CLI program - try running `heroku apps` to confirm it works. This API key is unique and private to you so do not share it. If you accidentally make it public then you can create a new one with _Regenerate API Key_.

