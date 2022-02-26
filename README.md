Check out my [Gists](https://gist.github.com/dark-teal-coder) for some code snippets :kissing_smiling_eyes:  

# Me Matters :girl: 

- 👋 Hi, I’m @dark-teal-coder
- 👀 I’m interested in :infinity: Mathematics, :octocat: coding, :statue_of_liberty: English, :film_strip: YouTube and :flight_departure: traveling ...
- 🌱 I’m currently learning JavaScript and R wtih solid knowledge of Python syntax already ...
- :computer: I have no CompSci degree ...
- :woman_technologist: I'm a woman in tech ... 
- I enjoy :sleeping_bed: and just do nothing ... 
- I want to see :maple_leaf: in person soon ... 

# Eating Matters :yum:

- :plate_with_cutlery: Favorite **foods**: :pancakes: :waffle: :hamburger: :pizza: :fondue: :bento: :curry: :ramen: :spaghetti: :oden: :sushi: :dumpling: :takeout_box: ... 
- :spoon: Favorite **desserts**: :ice_cream: :cookie: 	:cake: :custard: :doughnut: :cupcake: :honey_pot: ... 
- :clinking_glasses: Favorite **beverages**: :coffee: :tea: :cocktail: :cup_with_straw: :milk_glass: :tropical_drink: :bubble_tea: ... 

# Coding Matters :woman_technologist:

## Python `.py` & `.ipynb`
### Description
I've officially taken 2 Python courses before - one at undergraduate level and another at graduate level. I've also written some real-world applications in Python in one of my full-time jobs.  
- [x] IS2240 Python Programming for Business [A-]
- [x] CSCI E-7 Introduction to Python [A-]
### Syntax and Concepts
- basic syntax, e.g., variables, data types, string operations, arithmetic operators, assignment operators, comparison operators, logical operators, conditions, loops, functions, etc. 
- basic object-oriented programming (OOP) concepts, e.g., class/object, attributes, class methods, inner class, constructors, inheritance, etc.
- file handling
- exception handling
- recursion 
- lambda
### Applications
- regular expression (RegEx) with `re`
- data analysis with `pandas` 
- data visualization with `matplotlib` 
- web scrapping with `requests` & `BeautifulSoup`

## Java `.java` & `.class`
### Description
I've taken the following course which used Java in my undergraduate studies. Lectures 11 to 13 were on Formal Language and the others focused mainly on Java syntax and concepts. This cousre also touched on basic sorting algorithms. 
- [x] LT3233 Computational Linguistics [A]
### Syntax and Concepts
- basic syntax, e.g., variables, data types, string operations, arithmetic operators, assignment operators, comparison operators, logical operators, conditions, loops, functions, etc. 
- basic object-oriented programming (OOP) concepts, e.g., class/object, attributes, class methods, inner class, constructors, inheritance, encapsulation, polymorphism, etc.
- file handling
- exception handling
- recursion 
- basic sorting algorithms 

## HTML, CSS & JavaScript `.html` & `.css` & `.js`
### Description
I've taken the following undergraduate course that covers basic HTML and CSS syntax to create simple websites and JavaScript syntax to add interactivity to the websites many years ago. 
- [x] LT3210 Electronic Publishing [A]
### Syntax and Concepts
- ...

## R `.rmd`
### Description
I'm taking a R programming course at graduate level. There are one midterm and one final that together contribute to 80% of the final course grade. 
- [x] CSCI E-5a R Programming []
### Syntax and Concepts
- ...

# Git Matters

## Basic Steps to Get a Remote Repository on GitHub to Your Local Machine
Steps: 
1. Go to GitHub. 
2. Click into the remote repository that you want to get. 
3. Click the [Code] button. 
4. Select the [HTTPS] tab. 
5. Copy the HTTPS URL. 
6. Open a command-line interface (CLI). 
7. Change the directory to the one you want to put the entire remote repository in using the `cd` command followed by the directory path[^1]. 
8. Type `git clone` followed by the HTTPS URL you copied in Step 5[^2]. 
9. Press [ENTER]. 
[^1]: 
    A folder with the same name and structure as the remote repository will appear in the exact directory in which the `git clone` command is used on your local machine. 
[^2]: 
    It is unnecessary to use `git init` before `git clone`. The cloned respository already has `.git` folder inside it. 

## Basic Steps to Create a New Repository
Steps: 
1. Go to your profile page on GitHub. 
2. Select the [Repositories] tab. 
3. Click the [New] button. 
4. Name the new repository under "Repository name". 
5. Choose whether the repository should be [Public] or [Private]. 
6. Click the [Create repository] button[^3]. 
7. Open a command-line interface (CLI). 
8. Use the `cd` command followed by the directory path to navigate to the desired directory on your local machine[^4]. 
9. Use the `mkdir` command followed by the name of the remote repository to create the corresponding local repository. 
10. Use the `cd` command followed by the folder name to go inside it. 
12. Type `git init` to let Git start tracking the local repository. 
13. Use `git add .` to add all the files inside the local repository to the staging area[^5]. 
14. Use `git commit -m "commit message"` to capture a snapshot of the currently staged changes in the repository[^6]. 
15. Use `git branch -M main` to forcefully rename the default branch to "main"[^7]. 
16. Click into the remote repository.
17. Click the [Code] button. 
18. Select the [HTTPS] tab. 
19. Copy the HTTPS URL. 
20. Use the command `git remote add origin` followed by the HTTPS URL to add the remote repository's reference to the local repository[^8]. 
21. Use `git push -u origin main` to push the code from your local to the `main` branch of the remote repository at the HTTPS URL referenced by `origin`[^9]. 

[^3]: 
    You can also choose whether you want to add `README.md`, `.gitignore` and `LICENSE` filles to the newly created repository before clicking the [Create repository] button. 
[^4]: 
    You can also use the file manager application in your system to do this. 
[^5]: 
    This will direct Git to save a snapshot of the current project state into the commit history. 
[^6]: 
    This will tell Git to keep track of the progress and changes of the project so that you can recall or revert to the committed changes at a later date. 
[^7]:
    If you create a remote repository without adding a file (including `README.md`, `.gitignore` and `LICENSE`) inside, there will not be any branch yet. Once you add one or more files to the remote repository, the default branch will be `main` on GitHub. But when you `git add` files in the corresponding local repository, the default branch will be `master`. Therefore, you need to use `git branch -M main` to rename the local branch from `master` to `main` to match the remote repository branch setting. 
[^8]:
    `origin` references the HTTPS URL to the remote repository to push to from/pull from to the local repository. 
[^9]: 
    The `-u` options is a shorthand for `--set-upstream` which is used to map a local branch to a remote barnch. 

# References
- [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)

<br />

*Last modified date: Feb 26, 2022*

<!---
dark-teal-coder/dark-teal-coder is a special repository because its `README.md` (current file) appears on your GitHub profile. Click on [Preview] tab to take a look at your changes. 
--->
