
var readlineSync = require("readline-sync")

var number1= readlineSync.questionFloat("Please enter your first number: "  );
var number2= readlineSync.questionFloat("Please enter your second number: " );
var operation= readlineSync.question("Please enter the operation to perform: add, sub, mul, div: ");

function addTwoNumbers(num1,num2){
    return num1 + num2 
}
function subtractTwoNumbers(num1,num2){ 
    return num1 - num2
}
function multiplyTwoNumbers(num1,num2){
    return num1 * num2
}
function devideTwoNumbers(num1,num2){
    return num1 / num2
}

function calculator(number1,number2,operation){
if (operation == "add"){
    console.log("The result is: "+ addTwoNumbers(number1,number2))
}
else if (operation == "sub"){
    console.log("The result is: "+ subtractTwoNumbers(number1,number2))
}
else if (operation == "mul"){
    console.log("The result is: "+ multiplyTwoNumbers(number1,number2))
}
else if (operation =="div"){
    console.log("The result is: "+ devideTwoNumbers(number1,number2))
}else{
    console.log("Invalid Operation")
}
}
calculator(number1,number2,operation)
