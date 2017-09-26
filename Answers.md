- What is the complexity of each of the four search methods in terms of array or list size n?<br />
Both 'FindTeamPosition' methods increase in proportion to n (O(n)). <br />
This is due to the fact that the operations are run once for each item on the list (value of n) <br />
The same goes for FindTeamMinFunding, as it also runs its operations once per item <br />
FindTeamMidFundingFast is built on cutitng the search space in half, thus it's complexity  <br/>
is in porpotion to how many divisions by two it takes to narrow the search space (O(log(n))).<br />
<br />
<br /> 
- What happens in the case of binary search if the array is not sorted? <br />
The function will behave very unexpectedly. Possibly by stumbling onto clearly incorrect values,<br />
looping infinitely, or simply hitting a run-time error. A good check at the end or start of the loop  <br />
might catch most of these errors.<br />
<br />
<br /> 
- What is the purpose of constructor argument validity checking?<br />
Preventing runtime errors caused by methods attemtping operations on null values<br />
<br /> 
<br />
- What is the purpose of using the keyword `final` with variables and arguments?<br />
To mark those variables as constants, and make them unchangable in future <br />
Largely for structural reasons, and futureproofing against developer error <br />
<br />
<br />
- What are alternatives to using `Optional` and how do they compare?<br />
The normal 'bodged' solution would be to place a few if statements to check if <br />
the variables in question are null or real values. This is less desirable <br />
because it's clunky, takes up space, and has less utility than the 'Optional' class <br />