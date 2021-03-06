# pyflames
Python library to check two names and return their relationship status as per "FLAMES"

<h1><a href="/">Flames</a></h1>
      
<h2>How it works?<h2>
    <h3>What is FlamesGame?</h3>
    <br>
      FlamesGame is a relationship calculating algorithm famous between the youngsters. At the time of graduation everyone might heard about this and many of them tried out this secretly. Some took this as very serious also. So what FLAMES stance for?
      <br/>
      F - Friendship
      <br/>
      L - Love
      <br/>
      A - Affection
      <br/>
      M - Marriage
      <br/>
      E - Enemy
      <br/>
      S - Sister (Sibling)
    </p>
    <h3>How we can calculate the FLAMES?</h3>
    <p>
      It is very easy to explain with some example:
      <br/>
      Your name: <b>asd</b>
      <br/>
      Partner name: <b>abcd</b>
      <br/><br/>
      Mainly two steps are there:
    </p>
    <ol>
      <li>Get the flames count
        <ul>
          <li>Take the two names ('asd' and 'abcd')</li>
          <li>Remove the common characters (two common characters 'a', 'd') </li>
          <li>Get the count of the characters that are left (Removed a,d and the rest are s,b,c. So total 3.)</li>
        </ul>
      </li>
      <li>Get the flames result
        <ul>
          <li>We take FLAMES letters ('F', 'L', 'A', 'M', 'E', 'S')</li>
          <li>And start removing letters using the flames count we got.</li>
          <li>And the letter which last the process is the result.</li>
        </ul>
      </li>
    </ol>
    <p>
      In our example we got <b>flames count = 3</b>. So first we takes FLAMES.
      <br/>
      <b>FLAMES</b>
      <br/>
      Then we start count from left up to flames count 3. Then remove the letter which is in the position 3. In this case it is 'A'. So the letters become:
      <br/>
      <b>FLMES</b>
      <br/>
      Then we start count again from the letter which is removed ie, from 'M'. So the next character to remove is 'S'. So our letters become:
      <br/>
      <b>FLME</b>
      <br/>
      After next step:
      <br/>
      <b>FLE</b>
      <br/>
      Then:
      <br/>
      <b>FE</b>
      <br/>
      Last:
      <br/>
      <b>F</b>
      <br/>
      So the result is '<b>Friend</b>'.              
    </p>
  
  <br><h3> So it's as simple as that! </h3>
  
  <br><b>USAGE:</b><br>
  From packagename import package name <br>
  Create an instance of the class <br>
  Create variable and call the flames method referencing the instance that we created <br>
  
  <br><b>SYNTAX:</b><br>
  ```
  variable_name = pyflames()
  another_variable = variable_name.flames("name1","name2")
  print(another_variable)
  ```
  
  <br><b>EXAMPLE CODE:</b><br>
  
```
from pyflames import pyflames
word = pyflames()
status = word.flames("John Wick","Jennifer Aniston")
print(status)
```
