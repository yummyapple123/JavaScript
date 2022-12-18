# JavaScript
function logger() {
  console.log("My name is Van");
}
logger();
function fruitProcessor(apples, oranges) {
  console.log(apples, oranges);
  const juice = `Juice with ${apples} and apples and ${oranges} oranges`;
  return juice;
}
const appleJuice = fruitProcessor(3, 9);
console.log(appleJuice);
console.log(fruitProcessor(3, 9));
