# JavaScript - Ternary Operator
# instead of using if-else statements, ternary can be used to make the code shorter and convenient sometimnes, prompting user to enter the bill value between 50 and 300 to get the tip equals to 15% or else, the tip would be 20% of the total bill
let bill = Number(prompt("What is the bill value? "));
let tips;

console.log(
  bill >= 50 && bill <= 300 ? (tips = bill * 0.15) : (tips = bill * 0.2)
);
