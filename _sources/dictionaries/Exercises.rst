Multiple Choice Questions
---------------------------

.. mchoice:: Exercises_question9_1
  :practice: T
  :answer_a: fruit['grapes']
  :answer_b: fruit['grapes'] = 15
  :answer_c: insert 'grapes' in fruit
  :answer_d: 'grapes' = 15
  :correct: b
  :feedback_a: Try again! This line inserts 'grapes' as a key in the dictionary fruits with  no value.
  :feedback_b: Correct! This line inserts 'grapes' as a key in the dictionary fruits with  a value of 15.
  :feedback_c: Try again! This is not how to insert a key into a dictionary.
  :feedback_d: Try again! This line assigns 'grapes' with  a value of 15, but does not add the key in the dictionary fruits.


  Which line of code correctly initializes 'grapes' into the fruits dictionary?

  .. code-block:: python

     fruits = {'apples': 1, 'bananas': 4, 'pears': 17, 'oranges': 14}

.. mchoice:: Exercises_question9_2
   :practice: T
   :answer_a: ['Janice', 'John']
   :answer_b: ['Janice', 'Emily', 'Eleanor']
   :answer_c: ['John']
   :answer_d: ['Janice'] 
   :correct: c
   :feedback_a: Try again! John has a value greater than 5, but Janice does not.
   :feedback_b: Try again! None of these keys have a value that is greater than 5.
   :feedback_c: Correct! John is the only key that has a value greater than 5.
   :feedback_d: Try again! Janice has a value that is equal to 5, but not greater than 5.

   What prints when the following code is run?

   .. code-block:: python

      names = {'Janice': 5, 'Emily': 3, 'John': 7, 'Eleanor': 2}
      list_o_names = []
      for name in names:
          if names[name] > 5:
              list_o_names.append(name)
      print(list_o_names)

.. mchoice:: Exercises_question9_3
   :practice: T
   :answer_a: ['Emily', 'John', 'Erik']
   :answer_b: ['Janice', 'Emily', 'John']
   :answer_c: ['Janice', 'John', 'Erik']
   :answer_d: ['Janice', 'Emily', 'John', 'Erik']
   :correct: a
   :feedback_a: Correct! Erik is initialized to 22, and Emily is updated to 13, therefore these two entries are added to the list found in the prior question.
   :feedback_b: Try again! Emily and John now both have a value that is greater than 5, but Janice does not have a value that is greater than 5.
   :feedback_c: Try again! Erik and John have a value that is greater than 5, but Janice does not have a value that is greater than 5.
   :feedback_d: Try again! This is just a list of all the keys in the dictionary rather than the ones greater than 5.


   What does the following code print now that it has been updated?

   .. code-block:: python

      names = {'Janice': 5, 'Emily': 3, 'John': 7, 'Eleanor': 2}
      list_o_names = []

      names['Emily'] += 10
      names['Erik'] = 22

      for name in names:
          if names[name] > 5:
              list_o_names.append(name)
      print(list_o_names)

.. mchoice:: Exercises_question9_4
   :practice: T
   :answer_a: 5
   :answer_b: 10
   :answer_c: 9
   :answer_d: 12
   :correct: c
   :feedback_a: Try again! Make sure to properly count the number of times a letter counted more than twice.
   :feedback_b: Try again! Make sure to properly count the number of times a letter counted more than twice.
   :feedback_c: Correct! There are 9 letters in phrase that appear more than two times.
   :feedback_d: Try again! Only count the letters that appear more than twice and do not include the ones that only show up twice.

   What is the value of counter after the code is run to completion?

   .. code-block:: python

      phrase = "Cheese in Philadelphia is extraordinary according to Erik"

      counter = 0
      letters = {}
      for word in phrase.split():
          for letter in word:
              letter = letter.lower()
              if letter not in letters.keys():
                  letters[letter] = 0
              letters[letter] += 1
      for key in letters.keys():
          if letters[key] > 2:
              counter += 1

.. mchoice:: Exercises_question9_5
   :practice: T
   :answer_a: fruits.get(apples)
   :answer_b: fruits.get('apples', 0)
   :answer_c: fruits.get('apple')
   :answer_d: fruits.get(apples, 0)
   :correct: b
   :feedback_a: Try again! This incorrectly grabs the key and does not grab the value.
   :feedback_b: Correct! This correctly grabs the key as a string, and also includes a default value in case the key is not present in the dictionary.
   :feedback_c: Try again! This only grabs the key, but not the value.
   :feedback_d: Try again! This incorrectly grabs the key.

   Which line of code correctly grabs the value of the key 'apples'?

   .. code-block:: python

      fruits = {'bananas': 7, 'apples': 4, 'grapes': 19, 'pears': 4}

.. mchoice:: Exercises_question9_6
   :practice: T
   :answer_a: 10
   :answer_b: 4
   :answer_c: 6
   :correct: c
   :feedback_a: Try again! Remember, the get function grabs the number of 'o' in brontosaurus.
   :feedback_b: Try again! Remember, the get function grabs the number of 'o' in brontosaurus.
   :feedback_c: Correct! The .get() function grabs the value 2, and then 4 gets added to it to get 6.

   What value is printed once the code is run?

   .. code-block:: python

      word = 'brontosaurus'
      diction = {}
      for letter in word:
          if letter not in diction.keys():
              diction[letter] = 0
          diction[letter] += 1
     print(diction.get('o', 0) + 4)


.. mchoice:: Exercises_question9_7
   :practice: T
   :answer_a: jan, chuck, annie
   :answer_b: chuck, annie, jan
   :answer_c: annie, chuck, jan
   :correct: a, b, c
   :feedback_a: Correct! When written like this, they keys will not come out in any particular order. If you want them ordered, you have to use the sort function.
   :feedback_b: Correct! When written like this, they keys will not come out in any particular order. If you want them ordered, you have to use the sort function.
   :feedback_c: Correct! When written like this, they keys will not come out in any particular order. If you want them ordered, you have to use the sort function.

   What order do the keys print in after the following code is run? (Select all that apply)

   .. code-block:: python

      counts = {'chuck' : 1, 'annie' : 42, 'jan' : 100}
      for key in counts:
          print(key, counts[key])

.. mchoice:: Exercises_question9_8
   :practice: T
   :answer_a: import String
   :answer_b: import string
   :answer_c: import string module
   :answer_d: import String module
   :correct: b
   :feedback_a: Try again! The name of the module is written with a lower case s
   :feedback_b: Correct! This is the correct way to initialize the string module
   :feedback_c: Try again! The term module is implied when importing the string module
   :feedback_c: Try again! The name of the module is written with a lower case s and the term module is implied when importing the string module

   Which of the following is the correct way to initialize the string module?


.. mchoice:: Exercises_question9_9
   :practice: T
   :answer_a: True
   :answer_b: False
   :correct: b
   :feedback_a: Try again! These are two different words distinguished by the capital letter.

   :feedback_b: Correct! These are two different words distinguished by the capital letter.

   True or false? Python treats the words "Exciting" and "exciting" as the same word.

.. mchoice:: Exercises_question9_10
   :practice: T
   :answer_a: line.translate(str.maketrans(fromstr, tostr, deletestr))
   :answer_b: line.translate(fromstr, tostr, deletestr)
   :answer_c: line.translate(str.translate(fromstr, tostr, deletestr))
   :answer_d: line.maketrans(fromstr, tostr, deletestr)
   :correct: a
   :feedback_a: Correct! In order to use .translate(), you have to map the translation using the .maketrans() method.
   :feedback_b: Try again! In order to use .translate(), you have to map the translation using the .maketrans() method.
   :feedback_c: Try again! In order to use .translate(), you have to map the translation using the .maketrans() method not .translate().
   :feedback_d: Try again! .maketrans() is for mapping the translation, missing the .translate().



   Which line of code correctly uses the .translate() method?