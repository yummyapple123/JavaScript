# JavaScript
//CHALLENGE 1
// const avg = (score1, score2, score3) => (score1 + score2 + score3) / 3;
// const avgDolphins = avg(44, 23, 71);

// const avgKoalas = avg(65, 54, 49);
// // checkWinner
// function checkWinner(avgDolphins, avgKoalas) {
//   if (avgDolphins > avgKoalas * 2) {
//     console.log(`Dolphins win (${avgDolphins} vs ${avgKoalas})`);
//   } else if (avgKoalas > avgDolphins * 2) {
//     console.log(`Koalas win (${avgKoalas} vs ${avgDolphins})`);
//   } else {
//     console.log("No one wins!");
//   }
// }

// console.log(checkWinner(avgDolphins, avgKoalas));

// solution
const calcAverage = (a, b, c) => (a + b + c) / 3;

let scoreDolphins = calcAverage(44, 23, 71);
let scoreKoalas = calcAverage(65, 54, 49);
console.log(scoreDolphins, scoreKoalas);
const checkWinner = function (avgDolphins, avgKoalas) {
  if (avgDolphins >= avgKoalas * 2) {
    console.log(`Dolphins win the 🏆. ${avgDolphins} vs. ${avgKoalas}`);
  } else if (avgKoalas > avgDolphins * 2) {
    console.log(`Koalas win the 🏆. ${avgKoalas} vs. ${avgDolphins}`);
  } else {
    console.log("No one wins");
  }
};
checkWinner(scoreDolphins, scoreDolphins);
checkWinner(576, 111);

//test data 2
scoreDolphins = calcAverage(85, 54, 41);
scoreKoalas = calcAverage(23, 34, 27);
console.log(scoreDolphins, scoreKoalas);
checkWinner(scoreDolphins, scoreKoalas);
