Writing your first test
============

Why write tests?
---------------
Boozang allows you to write tests in natural language. This might seem more cumbersome than recording a test, but is very useful for test-driven or behavior-driven development, where you write the tests before the actual application code. It's also useful to allow non-technical people to be able to write tests. 

The Boozang test syntax
------------
The Boozang syntax aims to be as close to natural language as possible. The syntax comprises of an action keyword and a target element. The best way of getting started is simply recording a set of actions in your application and converting them to test instructions, and simply following suit. The full Boozang synatx reference can be found here (insert link here). 

Running a test
---------------
To run a test instruction the Boozang syntax needs to be converted to test ations. In order to do this you simply click the magic wand inside the tool, and choose "Generate actions based on descriptions". This will automatically convert each test instruction into an action and run the action. By running each action the Boozang tool is always working on the "current" state of the application so it's able to do more accurate interpretations of the Boozang syntax. This approach is vastly superior to stateless key-word driven test tools that has no information of the state of the application, which means the syntax will be very unforgiving to mistakes. 

Generating test instructions
---------------
Boozang also allows for automatic generation of test instructions. After a test has been recorded simply click on the magic wand and choose "Generate test instructions from actions" and the instructions will be generated. 

Updating your code
-----------------------------
After you have recorded a set of actions these are linked to the application code. As Boozang is based on natural language the tests are often very resilient to code updates. In the case where a code update is breaking a test, it could be worth autogenerate the test from the test syntax. Simply click on the magic wand to generate the test instructions and again to re-generate the actions and the test will be re-built based on your source code. 