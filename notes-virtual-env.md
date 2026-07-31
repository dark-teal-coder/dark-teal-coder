# How to Install a Virtual Environment Using Venv

Virtualenv is a tool to set up your Python environments. Since Python 3.3, a subset of it has been integrated into the standard library under the venv module. You can install venv to your host Python by running this command in your terminal:

```powershell
pip install virtualenv
```

To use venv in your project, in your terminal, create a new project folder, cd to the project folder in your terminal, and run the following command:

```powershell
python -m venv <virtual-environment-name>
```

When you check the new "projectA" folder, you will notice that a new folder called <virtual-environment-name> has been created. <virtual-environment-name> is the name of our virtual environment, but it can be named anything you want.

If we check the contents of <virtual-environment-name> for a bit, on a Windows, you will see a "Scripts" folder. You will also see scripts that are typically used to control your virtual environment, such as activate and pip to install libraries, and the Python interpreter for the Python version you installed, and so on. 

The "Lib" folder will contain a list of libraries that you have installed. If you take a look at it, you will see a list of the libraries that come by default with the virtual environment.

![virtual-env-folder.png](./images/virtual-env-folder.png)

# How to Activate the Virtual Environment

Now that you have created the virtual environment, you will need to activate it before you can use it in your project. On a Windows, to activate your virtual environment, run the code below:

```powershell
.\<virtual-environment-name>\Scripts\activate
```

This will activate your virtual environment. Immediately, you will notice that your terminal path includes env, signifying an activated virtual environment.

![activate-virtual-env.png](./images/activate-virtual-env.png)

# How to Check if the Virtual Environment is Working

First, we check the list of packages installed in our virtual environment by running the code below in the activated virtual environment. You will notice only two packages – pip and setuptools, which are the base packages that come default with a new virtual environment

```powershell
pip list
```

![pip-list-virtual-env.png](./images/pip-list-virtual-env.png)

Next, you can run the same code above in a new terminal in which you haven't activated the virtual environment. You will notice a lot more libraries in your host Python that you may have installed in the past. These libraries are not part of your Python virtual environment until you install them.

# How to Install Libraries in a Virtual Environment

To install new libraries, you can easily just pip install the libraries. The virtual environment will make use of its own pip, so you don't need to use pip3.

After installing your required libraries, you can view all installed libraries by using pip list, or you can generate a text file listing all your project dependencies by running the code below:

```powershell
pip freeze > requirements.txt
```

You can name this requirements.txt file whatever you want.

# Requirements File

Why is a requirements file important to your project? Consider that you package your project in a zip file (without the env folder) and you share with your developer friend.

To recreate your development environment, your friend will just need to follow the above steps to activate a new virtual environment.

Instead of having to install each dependency one by one, they could just run the code below to install all your dependencies within their own copy of the project:

```powershell
pip install -r requirements.txt
```

Note that it is generally not advisable to share your env folder, and it should be easily replicated in any new environment.

Typically your env directory will be included in a .gitignore file (when using version control platforms like GitHub) to ensure that the environment file is not pushed to the project repository.

## Requirements File Format

![requirements.txt-format.png](./images/requirements.txt-format.png)

# How to Deactivate a Virtual Environment

To deactivate your virtual environment, simply run the following code in the terminal:

```powershell
deactivate
```

![deactivate-virtual-env.png](./images/deactivate-virtual-env.png)

# Reference

- [How to Set Up a Virtual Environment in Python – And Why It's Useful](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/)
