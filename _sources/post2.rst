Posttest Problem 2
-------------------

Try to solve the following fix code problem.  You have five minutes to try to
solve it.  It is okay if you can't solve it, you will earn credit for trying to
solve it.

.. timed:: post-exa-2
   :timelimit: 300

   .. activecode:: find_extras_fix_timed
      :autograde: unittest
      :nocodelens:

      Fix the function ``two_cats`` below to return True if there are at least two adjacent "cat" strings in list ``pets``, otherwise return False.  For example, return ``True`` for ``['dog', 'cat', 'cat']`` since there are two adjacent items equal to 'cat' (at index 1 and 2) and ``False`` for ``['cat', 'dog', 'cat']`` since the 'cat' strings are not adjacent.

      ~~~~
      def two_cats(pets):
          i = 1
          while i < pets:
              if pets[i] = 'cat' and pets[i - 2] == 'cat':
                  return true
              i += 1
              return False

      ====
      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

          def testOne(self):
              self.assertEqual(two_cats(['dog', 'cat', 'cat']), True, "two_cats(['dog', 'cat', 'cat'])")
              self.assertEqual(two_cats(['dog', 'cat', 'dog', 'cat']), False, "two_cats(['dog', 'cat', 'dog', 'cat'])")
              self.assertEqual(two_cats(['cat', 'dog', 'cat']), False, "two_cats(['cat', 'dog', 'cat'])")
              self.assertEqual(two_cats(['cat', 'cat', 'dog']), True, "two_cats['cat', 'cat', 'dog'])")
              self.assertEqual(two_cats(['bird', 'fish', 'cat']), False, "two_cats(['bird', 'fish', 'cat'])")
              self.assertEqual(two_cats(['cat']), False, "two_cats(['cat'])")
              self.assertEqual(two_cats([]), False, "two_cats([])")
              self.assertEqual(two_cats(['cat', 'bird', 'fish', 'cat']), False, "two_cats([['cat', 'bird', 'fish', 'cat']])")
              self.assertEqual(two_cats(['fish', 'cat', 'cat', 'fish', 'fish']), True, "two_cats(['fish', 'cat', 'cat', 'fish', 'fish']")
              self.assertEqual(two_cats(['cat', 'bird', 'bird', 'cat']), False, "two_cats(['cat', 'bird', 'bird', 'cat'])")

      myTests().main()

.. poll:: find_extras_fix_timed_poll
    :allowcomment:
    :option_1: Very, very low mental effort
    :option_2: Very low mental effort
    :option_3: Low mental effort
    :option_4: Rather low mental effort
    :option_5: Neither low nor high mental effort
    :option_6: Rather high mental effort
    :option_7: High mental effort
    :option_8: Very high mental effort
    :option_9: Very, very high mental effort
    :results: instructor

    In solving the preceding problem I invested:
