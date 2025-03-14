let age = 21;
let birthYear = new Date().getFullYear() - age;
console.log("Age:", age, "Birth Year:", birthYear);
function testScope() {
    let x = 10;
}
console.log(typeof x); // Undefined (x is not accessible outside the function)

let num1 = 10, num2 = 5;
console.log("Sum:", num1 + num2);
console.log("Difference:", num1 - num2);
console.log("Product:", num1 * num2);
console.log("Quotient:", num1 / num2);

let strNum = "123";
let convertedNum = Number(strNum);
console.log("Converted to Number:", convertedNum, "Back to String:", String(convertedNum));

let number = 7;
console.log(number % 2 === 0 ? "Even" : "Odd");

let personAge = 18;
if (personAge < 13) {
    console.log("Child");
} else if (personAge < 20) {
    console.log("Teenager");
} else if (personAge < 60) {
    console.log("Adult");
} else {
    console.log("Senior");
}

let checkNum = -5;
console.log(checkNum > 0 ? "Positive" : checkNum < 0 ? "Negative" : "Zero");

let trafficLight = "red";
switch (trafficLight) {
    case "red": console.log("Stop"); break;
    case "yellow": console.log("Ready"); break;
    case "green": console.log("Go"); break;
    default: console.log("Invalid color");
}

for (let i = 1; i <= 10; i++) {
    console.log(i);
}

let userInput;
while (userInput !== "stop") {
    userInput = prompt("Enter something (type 'stop' to end):");
}

let i = 1;
do {
    console.log(`5 x ${i} = ${5 * i}`);
    i++;
} while (i <= 10);

function greet(name) {
    console.log(`Hello, ${name}!`);
}
greet("Mahnoor");

function sum(a, b) {
    return a + b;
}
console.log(sum(3, 7));

function findMax(numbers) {
    return Math.max(...numbers);
}
console.log(findMax([3, 7, 2, 8, 5]));

const greetArrow = name => console.log(`Hello, ${name}!`);
greetArrow("Mahnoor");

const square = num => num * num;
console.log(square(4));

const findLongString = arr => arr.find(str => str.length > 5);
console.log(findLongString(["apple", "banana", "kiwi", "strawberry"]));

let numbersArr = [1, 2, 3, 4, 5];
let sumArr = numbersArr.reduce((acc, val) => acc + val, 0);
console.log("Sum of array elements:", sumArr);

let names = ["Ali", "Ahmed", "Zainab", "Muhammad", "Fatima"];
let longestName = names.reduce((a, b) => (a.length > b.length ? a : b));
console.log("Longest name:", longestName);

let numArray = [1, 2, 3, 2, 4, 1, 5];
let uniqueNums = [...new Set(numArray)];
console.log("Unique numbers:", uniqueNums);
