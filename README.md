# import-js
- import
- ES6 module syntax also introduces the import keyword for importing objects. In our order.js example, we import an object like this:
- 
- import Menu from './menu';
- The import keyword begins the statement.
- The keyword Menu here specifies the name of the variable to store the default export in.
- from specifies where to load the module from.
- './menu' is the name of the module to load. When dealing with local files, it specifically refers to the name of the file without the extension of the file.



**#### QQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQQ**

- In missionControl.js we’ll use the module Airplane to display the fuel capacity of both our airplanes.
- 
- Use the import keyword to import the Airplane module.
- 
- Checkpoint 2 Passed
- 
- Hint
- import Airplane from './airplane';
- - Define a function displayFuelCapacity().
- 
- Checkpoint 3 Passed
- 
- Hint
- function displayFuelCapacity() {
- }
- - Within the body of the displayFuelCapacity function, use forEach() to iterate over the Airplane.availableAirplanes array.
- 
- The forEach() should take an anonymous function as a parameter. We’ll add more in the next step.
- 
- Checkpoint 4 Passed
- 
- Hint
- function displayFuelCapacity() {
-   Airplane.availableAirplanes.forEach(function(){});
- }
- - Pass the anonymous function you created in the last step a parameter of element.
- 
- Checkpoint 5 Passed


Hint
function displayFuelCapacity () {
 Airplane.availableAirplanes.forEach(function(element) {
  });
}
5.
Within the displayFuelCapacity function, use console.log() to output the element’s name and its fuel capacity. The output should look like this:

'Fuel Capacity of + (element name) : + (element fuelCapacity)'
Checkpoint 6 Passed

Hint
For this checkpoint, make sure to use single quotes like the code below:

function displayFuelCapacity() {
  Airplane.availableAirplanes.forEach(function(element){
  console.log('Fuel Capacity of ' + element.name + ': ' + element.fuelCapacity);
  });
}
 
6.
Call the displayFuelCapacity function.

Checkpoint 7 Passed

Hint
displayFuelCapacity();
