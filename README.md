# JavaScript
Function declaration: function that can be used b4 it’s declared
function calcAge(birthYear){
	Return 2037 - birthYear;
}
Function Expression: essentially a function value stored in a variable
function calcAge = function (birthYear){
	Return 2037 - birthYear;
}
Arrow function great for a quick one-line functions. Has no this keyword(more later)
const calcAge = birthYear => 2037 - birthYear;
