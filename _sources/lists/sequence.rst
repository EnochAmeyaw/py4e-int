A list is a sequence
--------------------
.. index::
    single: Element
    single: Sequence
    single: Item
    single: Assignment
    single: Nested List
    pair: Empty; List

Like a string, a *list* is a sequence of values. In a
string, the values are characters; in a list, they can be any type. The
values in list are called *elements* or sometimes
*items*.

There are several ways to create a new list; the simplest is to enclose
the elements in square brackets ("[" and "]"):

.. code-block:: python

   [10, 20, 30, 40]
   ['crunchy frog', 'ram bladder', 'lark vomit']


The first example is a list of four integers. The second is a list of
three strings. The elements of a list don't have to be the same type.
The following list contains a string, a float, an integer, and (lo!)
another list:

.. code-block:: python

   ['spam', 2.0, 5, [10, 20]]


A list within another list is *nested*.

A list that contains no elements is called an empty list; you can create
one with empty brackets, ``[]``.

As you might expect, you can assign list values to variables:

.. activecode:: listExamples
    :caption: Examples of lists.

    cheeses = ['Cheddar', 'Edam', 'Gouda']
    numbers = [17, 123]
    empty = []
    print(cheeses, numbers, empty)

.. mchoice:: listSeq_MC_tf
    :practice: T
    :answer_a: A list cannot contain zero elements.
    :answer_b: A list can contain only integer items.
    :answer_c: A list has to contain items of the same type.
    :answer_d: A list can contain a list of items.
    :correct: d
    :feedback_a: Try Again! A list that contains no elements is called an empty list; you can create one with empty brackets.
    :feedback_b: Try Again! lists can contain any combination of items, even other lists!
    :feedback_c: Try Again! The elements of a list don�t have to be the same type.
    :feedback_d: Correct! A list within another list is nested.

    Which of the following is true about lists?

.. mchoice:: listSeq_MC_length
    :practice: T
    :answer_a: 1
    :answer_b: 3
    :answer_c: 4
    :answer_d: 5
    :correct: c
    :feedback_a: There is only one number in the list, but that is not the length.
    :feedback_b: There are three strings in the list, but that is not the length.
    :feedback_c: There are 4 items in this list (three strings and a number) making the length 4.
    :feedback_d: The value of the number in this list is 5, but that is not the length.

    What is the length of the list [“Sue”,”Maria”,5,”Erica”]?

.. fillintheblank:: listSeq_fill1
    :practice: T

    A list within another list is said to be __________.

    - :[Nn]ested: A list within another list is nested.
      :.*: Go back and reread the text.
