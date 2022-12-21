# JavaScript
const jonasArray = [
  "Jonas",
  "Schmedtmann",
  2037 - 1991,
  "teacher",
  ["Michael", "Peter", "Steven"],
];

//object jonas has 5 properties, 5 keys with values
const jonas = {
  firstName: "Jonas",
  lastName: "Schmedtmann",
  age: 2037 - 1991,
  job: "teacher",
  friends: ["Michael", "Peter", "Steven"],
};
console.log(jonas);
//Dot notation
console.log(jonas.lastName); //print out last name
//bracket notation
console.log(jonas["lastName"]);
// ---------------------------------
const nameKey = "Name";
console.log(jonas["first" + nameKey]);
console.log(jonas["last" + nameKey]);

const interestedIn = prompt(
  "What do you want to know about Jonas? Choose between firstName, lastName, age, job and friends"
);

if (jonas[interestedIn]) {
  console.log(jonas[interestedIn]);
} else {
  console.log(
    "Wrong request!, between firstName, lastName, age, job and friends"
  );
}
jonas.location = "Portugal";
jonas["twitter"] = "@jonasschmedtman";
console.log(jonas);

//challenge, print the sentence below without hard-coding, using dot notation
// Jonas has 3 friends, and his best bud is Michael,
console.log(
  "Jonas has " +
    jonas.friends.length +
    " friends, and his best friend is called " +
    jonas.friends[0]
);
//solution
console.log(
  `${jonas.firstName} has ${jonas.friends.length} friends, and his best friend is called ${jonas.friends[0]}`
);


/* Object Method with 'this' keyword */
const jonas = {
  firstName: "Jonas",
  lastName: "Schmedtmann",
  age: 2037 - 1991,
  job: "teacher",
  friends: ["Michael", "Peter", "Steven"],
  hasDriverLIcense: true,

  // calcAge: function (birthYear) {
  //   return 2037 - birthYear;
  // },
  calcAge: function () {
    console.log(this);
    return 2037 - this.birthYear;
  },
};

console.log(jonas.calcAge());
// console.log(jonas["calcAge"](1991));


//THE FOR LOOP
//print a sentence 10 times
console.log("lifting weights repitition 1 😀");
for (let i = 1; i <= 10; i++) {
  console.log("hello there");
}
