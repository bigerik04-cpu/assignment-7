// Personal Taste Tracker

let favoriteFoods = ["tacos", "pizza", "wings", "steak", "burgers"];

let popularFoods = [
  "pizza", "burgers", "tacos", "sushi", "pasta",
  "fries", "chicken", "steak", "ice cream", "salad",
  "mac and cheese", "ramen", "burritos", "hot dogs", "nachos",
  "donuts", "pancakes", "waffles", "cookies", "brownies",
  "sandwiches", "grilled cheese", "quesadillas", "fried rice", "shrimp",
  "lobster", "mashed potatoes", "corn", "green beans", "biscuits",
  "apple pie", "banana pudding", "cheesecake", "meatloaf", "gumbo",
  "jambalaya", "pho", "curry", "dumplings", "fish",
  "bbq ribs", "pulled pork", "chili", "omelet", "cereal",
  "bagels", "muffins", "spaghetti", "lasagna", "soup"
];

console.log("My favorite foods:");
console.log(favoriteFoods);

console.log("First favorite food:", favoriteFoods[0]);
console.log("Last favorite food:", favoriteFoods[favoriteFoods.length - 1]);

console.log("Loop through favorite foods:");
for (let i = 0; i < favoriteFoods.length; i++) {
  console.log(favoriteFoods[i]);
}

function describeFood(food) {
  console.log("One of my favorite foods is " + food + ".");
}

describeFood("tacos");
describeFood("steak");

if (favoriteFoods.includes("pizza")) {
  console.log("Pizza is one of my favorite foods.");
} else {
  console.log("Pizza is not one of my favorite foods.");
}

if (favoriteFoods.length > popularFoods.length) {
  console.log("My favorite foods list is longer than the popular foods list.");
} else if (favoriteFoods.length < popularFoods.length) {
  console.log("The popular foods list is longer than my favorite foods list.");
} else {
  console.log("Both arrays are the same length.");
}

console.log("Foods that appear in both arrays:");
for (let i = 0; i < favoriteFoods.length; i++) {
  if (popularFoods.includes(favoriteFoods[i])) {
    console.log(favoriteFoods[i]);
  }
}
