
## How to use the Random Module in Python ?
*  The **random module** provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.For example , when we want the computer to pick a random number in a given range or pick a random element from a list, pick a random card from a deck, flip a coin etc
* **The Random module contains some very useful functions** :
1. **Randint** >> to generate random integer and this function accepts two parameters: a lowest and a highest number.
  * **Example :**
```
import random
print random.randint(0, 5)
```
  * This will output either 1, 2, 3, 4 or 5.

2. **Random** >> to generate random number "float" between 0 and 1, If you want a larger number, you can multiply it.
  * **Example** :
```
import random
random.random() * 100
```
3. **Choice** >> to generate a random value from the sequence sequence.
The choice function can often be used for choosing a random element from a list.
If seq is empty, raises IndexError.
  * **Example** :
```
import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)
```
4. **Shuffle** : The shuffle function, shuffles the elements in list in place, so they are in a random order.
  * **Example**:
```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
```
5. **Randrange** >> to generate a randomly selected element from range(start, stop, step)
  * **Example**:
```
import random
for i in range(3):
    print random.randrange(0, 101, 5)
```
## What is Risk Analysis in Software Testing and how to perform it?
*  In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.
* **Why use Risk Analysis?** : When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.
* **Example of possible risks list** :
1. Use of new hardware
2. Use of new technology
3. Use of new automation tool
4. The sequence of code
5. Availability of test resources for the application

* There are certain risks that are unavoidable such as the time that you allocated for testing ,a defect leakage due to the complexity or size of the application ,urgency from the clients to deliver the project, or Incomplete requirements.In such cases, you have to tackle the situation with care by : 
  1. Conduct Risk Assessment review meeting
  2. Use maximum resources to work on high-risk areas
  3. Create a Risk Assessment database for future use
  4. Identify and notice the risk magnitude indicators: high, medium, low.
      **Note** :
     **High**: means the effect of the risk would be very high and non-tolerable.The company might face loss.         **Medium**: it is tolerable but not desirable.The company may suffer financially but there is a limited risk.  
      **Low**: it is tolerable. There lies little or no external exposure or no financial loss.
* **Risk Identification**
There are different sets of risks included in the risk identification process. Those are as follows:

1. **Business Risks**: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.
2. **Testing Risks**: You should be well acquainted with the platform you are working on, along with the software testing tools being used.
3. **Premature Release Risk**: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required
4. **Software Risks**: You should be well versed with the risks associated with the software development process.

* **The perspective of Risk Assessment** : There are three perspectives of Risk Assessment:
1. **Effect** – To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.
2. **Cause** – To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.
3. **Likelihood** – To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.

* There are three steps to perform risk analysis :
 1. Searching the risk
 2. Analyzing the impact of each individual risk
 3. Measures for the risk identified

## Big O : 
 * represent how time scales with respect to some input values 


# A quick intro to Dependency Injection: what it is, and when to use it :
* Dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service).
* **There are basically three types of dependency injection**:
 1. constructor injection: the dependencies are provided through a class constructor.
 2. setter injection: the client exposes a setter method that the injector uses to inject the dependency.
 3. interface injection: the dependency provides an injector method that will inject the dependency into any client passed to it.Clients must implement an interface that exposes a setter method that accepts the dependency.
* The dependency injection’s responsibility to: Create the objects , Know which classes require those objects And provide them all those objects
* Benefits of using DI are : Helps in Unit testing, Boiler plate code is reduced, as initializing of dependencies is done by the injector component, Extending the application becomes easier,Helps to enable loose coupling, which is important in application programming.
* Disadvantages of DI : It’s a bit complex to learn, and if overused can lead to management issues and other problems, Many compile time errors are pushed to run-time, Dependency injection frameworks are implemented with reflection or dynamic programming ,This can hinder use of IDE automation, such as “find references”, “show call hierarchy” and safe refactoring.
