# Addition

Scenario: Add two numbers
  
  Given I have a calculator and two numbers

  When I enter "number 1" and press "+" button
and enter "number 2" and press "=" button
  
  Then I see the result of addition

Scenario: Add more numbers
  
  Given I have a calculator and more than two numbers
  
  When I enter "number 1" and press "+" button
and enter "number 2" and press "+" button
and so on and press "=" button
  
  Then I see the result of addition
  
Scenario: Result is too large to display
  
  Given I have a calculator and two large numbers
  
  When I enter "number 1" and press "+" button
and enter "number 2" and press "=" button
  
  Then I see rounded off result
  
Scenario: Numbers can be negative
  
  Given I have a calculator and two numbers both negative
  
  When I enter "- number 1" and enter "- number 2"
and press "=" button
  
  Then I see the result of addition (negative)
  
Scenario: Numbers can be fraction

  Given I have a calculator and two numbers both fractions
  
  When I enter "number 1" and press "+"
and enter "number 2" with and press "="
  
  Then I see result of addition (decimal)
  
Scenario: Numbers can be irrational
  
  Given I have a calculator and two irrational numbers
  
  When I enter "number 1" and press "+"
and enter "number 2"
  
  Then I see result of addition
  
Scenario: Length of each number
  
  Given I have a calculator and two long numbers
  
  When I enter number 1
  
  Then calculator does not let me enter further
  
Scenario: If "number 1" or "number 2" is not entered
  
  Given I have a calculator with two numbers
  
  When I do not enter "number 1" or enter "number 1"
and press "+" and do not enter "number 2"
  
  Then calculator will wait for input
  
Scenario: If the number is real/complex
  
  Given (state the initial condition)
  
  When (state the event)
  
  Then (state the effect)
  
Scenario: If we are in between some operation
  
  Given (state the initial condition)
  
  When (state the event)
  
  Then (state the effect)
