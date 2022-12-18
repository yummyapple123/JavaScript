# JavaScript
//Function declaration
function calcAge1(birthyear) {
  return 2037 - birthyear;
}

const age1 = calcAge1(1993);
console.log(age1);
//function expression
//an expression produces a value
const calcAge2 = function (birthYear) {
  return 2037 - birthYear;
};
const age2 = calcAge2(1993);
console.log(age1, age2);
