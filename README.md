# JavaScript

//Array operations(methods)
const friends = ["Michael", "Steve", "Peter"];
const newLength = friends.push("Jay"); //add element to the end
console.log(friends);
console.log(newLength);

friends.unshift("John"); //add element to the start
console.log(friends);

friends.pop();
console.log(friends); //remove last element

friends.shift(); //remove first element
console.log(friends);

console.log(friends.indexOf("Steve"));
console.log(friends.indexOf("Van")); //-1 cuz not in the array

console.log(friends.includes("Steve")); //true
console.log(friends.includes("Van")); //false
friends.push(23);

if (friends.includes("Peter")) {
  console.log("You have a friend called Peter");
}

//Challenge
const calcTip = function (bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;
};
const bills = [125, 553, 44];
const tips = [calcTip(bills[0]), calcTip(bills[1]), calcTip(bills[2])];
const totals = [bills[0] + tips[0], bills[1] + tips[1], bills[2] + tips[2]];
console.log(bills, tips, totals);
