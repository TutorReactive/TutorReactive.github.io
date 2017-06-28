The Age Calculator

Forgot how old you are? Calculate it!

Write a function named calculateAge that:
takes 2 arguments: birth year, current year.
calculates the 2 possible ages based on those years.
outputs the result to the screen like so: "You are either NN or NN"
Call the function three times with different sets of values.
Bonus: Figure out how to get the current year in JavaScript instead of passing it in.

function calculateAge(birthYear, currentYear) {
    var age = currentYear - birthYear;
    console.log('You are either ' + age + ' or ' + (age - 1));
}

calculateAge(1984, 2012);
calculateAge(1988, 2012);
calculateAge(1982, 2012);



The Lifetime Supply Calculator

Ever wonder how much a "lifetime supply" of your favorite snack is? Wonder no more!

Write a function named calculateSupply that:
takes 2 arguments: age, amount per day.
calculates the amount consumed for rest of the life (based on a constant max age).
outputs the result to the screen like so: "You will need NN to last you until the ripe old age of 100"
Call that function three times, passing in different values each time.
Bonus: Accept floating point values for amount per day, and round the result to a round number.
See Solution 

function calculateSupply(age, numPerDay) {
  var totalNeeded = (numPerDay * 365) * (100 - age);
  var message = 'You will need ' + totalNeeded + ' cups of tea to last you until the ripe old age of 100';
  console.log(message);
}

calculateSupply(28, 36);
calculateSupply(28, 2.5);
calculateSupply(28, 400);



The Fortune Teller

Why pay a fortune teller when you can just program your fortune yourself?

Write a function named tellFortune that:
takes 4 arguments: number of children, partner's name, geographic location, job title.
outputs your fortune to the screen like so: "You will be a X in Y, and married to Z with N kids."
Call that function 3 times with 3 different values for the arguments.
See Solution 

function tellFortune(jobTitle, location, partner, numKids) {
    var future = 'You will be a ' + jobTitle + ' in ' + location + ' and married to ' +
   partner + ' ' + ' with ' + numKids + ' kids.';
    console.log(future);
}

tellFortune('bball player', 'spain', 'Shaq', 3);
tellFortune('stunt double', 'Japan', 'Ryan Gosling', 3000);
tellFortune('Elvis impersonator', 'Russia', 'The Oatmeal', 0);




The Geometrizer

Create 2 functions that calculate properties of a circle, using the definitions here.

Create a function called calcCircumfrence:

Pass the radius to the function.
Calculate the circumference based on the radius, and output "The circumference is NN".
Create a function called calcArea:

Pass the radius to the function.
Calculate the area based on the radius, and output "The area is NN".
See Solution 

function calcGeometry(radius) {
  var circumference = Math.PI * 2*radius;
  console.log("The circumference is " + circumference);
  var area = Math.PI * radius*radius;
  console.log("The area is " + area);
}
