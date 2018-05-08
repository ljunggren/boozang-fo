Test Types
==========

Different kinds of tests
------------------------
Boozang currently supports four different test types: Atomic, Functional, Composite and Bugs, These are actually very similar technically, but are conceptually different. The difference in icon also helps you to quickly classify which kind of test it is. 


Atomic Tests
------------
Atomic tests are building block for higher other tests. The atomic tests is usually comprised of a single action, such as Add Item or Delete Item. One thing that is notably different with atomic tests is that when being recorded they doesn´t relaod the URL, but assume that the test window is already at the right state. This makes them very fast to run, and ideal to stich together to form more complex functions. 

Function Tests
--------------
Function tests perform a function and usually cleans up after themselves. Function tests usually maps to requirements and a function tests, such as Item Search, might have data provisioning actions tied to it. In the example above, the Item Search test have calls a number of Atomic tests, such as Add Item and Delete Item.

Composite Tests
---------------
Composite tests are more complex tests, that stiches together atomic or unit tests. They are also used to build test suites, calling a list of function tests. As they are functionally very similar, it´s up to the test team how to best make use of the classification, and where the line between function and composite test should be drawn.

Bugs
----
Bugs are used to highlight a (usually visual) bug in the application. Becuase a failed test run can also denote a bug, the bug classification is usually used to point out a discrepancy using the Comment action. A typical Bug could be pointing out an incorrectly rendered image or an editorial problem, and allows one team member to communicate this to another team member without writing a bug report. This allows for quick turn-around of issues that can often be hard to reproduce when done manually. 