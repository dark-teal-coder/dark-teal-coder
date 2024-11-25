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
