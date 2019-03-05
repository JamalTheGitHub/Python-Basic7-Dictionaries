# Python Basic 7 Dictionaries

Prerequisite => From this tutorial onwards, it is expected that you have the following extensions in your Visual Studio Code;

1)Code Runner 2)Python

If you want to know more on how to get Python on Visual Studio Code, google it.

First thing first, create a file called called whatever you want it to be called and save it as ".py". For example like this, "python_tutorial.py". Navigate to that file and do your coding there.

================================================================================================

<h3>Dictionaries</h3>

What are <strong>dictionaries</strong>? Well you can think of it as a look up table. Another way of looking at it is <strong>key value pairs</strong>. Lets start by creating a <strong>dictionary</strong> to further understand it.

    d = {}

Now when we run this code, we just defined a <strong>dictionary</strong>. However, our dictionary is empty because we have not assign any key or values yet. Note that this <strong>dictionary</strong> is assigned to <strong>variable d</strong>. This means that a dictionary is not attached to a specific kind of variable as it can be anything. Another way to write the same thing is as follows;

    d = dict()

However, for now, we will use the <strong>d = {}</strong> method. Now that we have defined a dictionary, lets start by adding key value pairs to it. This can be accomplished by writing this line of code;

    d["James"] = 20

This line of code means to add <strong>"James"</strong> as <strong>key</strong> and the number associated to <strong>"James"</strong> is the </strong>value</strong> to the dictionary that we just created. Now <strong>print</strong> it and see what happens?

    print(d)

You will see something like <strong> {'James': 20}</strong> as the output. Okay, how about if we want to predefine the dictionary with our own set of keys and values? Well, lets declare another <strong>dictionary</strong> and add <strong>key value pairs</strong> to it;

    e = {"Eric": 15, "Monica": 18, "Ezzy": 20}
    print(e)

That is how you pre-defined a dictionary. Now, how would we want to select a particular <strong>key value pair</strong>? Well just like this;

    print(e["Monica"])

And just like that. What happen is that you select the <strong>key</strong> and it would print out the <strong>value</strong> associated with that <strong>key</strong>. The outcome of our example should give the output of <strong>18</strong>. Besides that, you can also change the <strong>value</strong> of the <strong>key</strong> by simply adding a new <strong>value</strong> to it like;

    e["Monica"] = 20

<strong>Print</strong> it again and see the <strong>value</strong> is now <strong>20</strong>.

NOTE that the <strong>values</strong> can be any type BUT the <strong>keys</strong> can only be a few type. Most commonly, <strong>keys</strong> are <strong>strings</strong> or <strong>numbers</strong>. In python, you can also mix different type of keys. Here is an example;

    e[5] = 50
    print(e[5])

Once you run the code, you will see that the output is <strong>50</strong>. Okay now that we have grasp the concept of <strong>dictionaries</strong>, lets think on how to iterate over the <strong>key value pairs</strong>. Sometimes if you forgot or do not know how to do such codes but you already have the concept of it, the best way is to <strong>google</strong> it. However, be careful when you <strong>google</strong> because depending on the version of your <strong>Python</strong> or any other <strong>programming language</strong>, older solutions or codes cannot be used anymore.

Now, for the purpose of this tutorial, I already know how to do it BUT it does not hurt if you <strong>google</strong> it yourself to sharpen your <strong>googling</strong> skills. Here is how we are going to iterate with Python 3.x where x is just the number after the decimal of version 3 Python;

    for key, value in e.items():
      print(key)
      print(value)

Just like that, you will iterate over the <strong>keys</strong> and <strong>values</strong> inside the <strong>dictionary</strong>.


================================================================================================

Alright, it is time for an exercise to see if you understand this topic! Okay, given what we have learnt so far, I need you to iterate this <strong>dictionary</strong>;

    d = {"James": 18, "Lisa": 17, "Jane": 16, "Andy": 19, "Antonio": 20}

Assuming the values are age, iterate the <strong>dictionary</strong> in such a way that only <strong>18 and above</strong> will be the outcome.
