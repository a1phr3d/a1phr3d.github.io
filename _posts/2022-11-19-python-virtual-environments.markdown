---
layout: post
title:  "Python Virtual Environments"
permalink: "/posts/2022-11-19-python-virtual-environments"
date:   2022-11-19 20:14:00 -0500
categories: 
---


Visit [dataquest][data-quest] for a more in-depth overview of what python virtual environments are, as well as 
what advantages they promise. 


<h3 style = "margin-top: 1.8em">Creating a Python Virtual Environment (Windows)</h3>
<!-- #; font-size: 14px -->
{% highlight ruby %}
py -m venv ['/path/to/new/virtual/environment']
{% endhighlight %}

<h3 style = "margin-top: 1.8em">Activating a Python Virtual Environment</h3>
{% highlight ruby %}
['/path/to/new/virtual/environment']\scripts\activate
{% endhighlight %}

<h3 style = "margin-top: 1.8em">Installing Packages in a Python Virtual Environment</h3>
By default, only pip and setup tools are initially installed. To check the pre-installed packages:
{% highlight ruby %}
pip list
{% endhighlight %}

To upgrade pip:
{% highlight ruby %}
py -m pip install --upgrade pip
{% endhighlight %}

To install new packages:
{% highlight ruby %}
py -m pip install pandas
{% endhighlight %}

<h3 style = "margin-top: 1.8em">Reproducing a Python Virtual Environment</h3>
You first need to list all the dependencies installed. Export the package list into a requirements.txt file
{% highlight ruby %}
pip freeze > requirements.txt
{% endhighlight %}
Create a virtual environment, activate it, and then run:
{% highlight ruby %}
pip install -r requirements.txt
{% endhighlight %}

Note: 
> If you’re going to add your project to a Git repository, never add its virtual environment folder to the repository. The only thing you need to add is the requirements.txt file.

> A Python project folder contains source code that runs in a virtual environment. On the other hand, a virtual environment is a folder that contains the Python interpreter, packages, and tools like pip. So, the best practice is to keep them separate and never put your project files in a virtual environment folder. 

<h3 style = "margin-top: 1.8em">Deactivating a Python Virtual Environment</h3>
{% highlight ruby %}
deactivate
{% endhighlight %}

<h3 style = "margin-top: 1.8em">Deleting a Python Virtual Environment</h3>
If you want to delete a virtual environment, you can simply delete its folder, no uninstall required
{% highlight ruby %}
rm -rf ['/path/to/new/virtual/environment']
{% endhighlight %}

<h3 style = "margin-top: 1.8em">Use Python Virtual Environments in Visual Studio Code</h3>
First, ensure you have created and activated a virtual environment.<br>
Then navigate to your project folder in the terminal <br> 
and run the following command:
{% highlight ruby %}
code .
{% endhighlight %}

The command above will open the project folder in VS Code. If the command above doesn’t work, open VS code, press command + shift + P, to open the Command Palette, type shell command and select Install ‘code’ command in PATH. Now, create a Python file, and name it my_script.py. The last step is to select the virtual environment using the Python: Select Interpreter command from the Command Palette. To do so, press Command + shift + P, and type Python, and choose Select Interpreter.
The Python: Select Interpreter command displays all available environments. 



[data-quest]:  https://www.dataquest.io/blog/a-complete-guide-to-python-virtual-environments/