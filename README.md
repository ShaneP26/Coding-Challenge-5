// Task 1 - Customer Profile

// Declare the customer object
const customer = {
    name: "John Doe",
    age: 35,
    email: "john.doe@email.com"
};

// Log each property using template literals
console.log(`Customer Name: ${customer.name}`);
console.log(`Customer Age: ${customer.age}`);
console.log(`Customer Email: ${customer.email}`);
# Coding-Challenge-5
// Task 2 - Order Details Method

// Declare the order object
const order = {
    orderId: 12345,
    totalAmount: 150,
    status: "Processing",

    // Method to display order details
    displayOrder: function() {
        console.log(`Order ID: ${this.orderId}`);
        console.log(`Total Amount: $${this.totalAmount}`);
        console.log(`Status: ${this.status}`);
    }
};

// Call the method to log order details
order.displayOrder();
// Task 3 - Shopping Cart Array Manipulation

// Declare an array with three product names
let cartItems = ["Laptop", "Phone", "Headphones"];

// Add a new product at the end
cartItems.push("Tablet");

// Remove the last item
cartItems.pop();

// Add an item at the beginning
cartItems.unshift("Smartwatch");

// Remove the first item
cartItems.shift();

// Log the final cart items
console.log("Final Cart Items:", cartItems);
// Task 4 - Price Adjustments with Map Method

// Declare the prices array
let prices = [100, 200, 300];

// Apply a 10% discount using map()
let discountedPrices = prices.map(price => price * 0.9);

// Log the new discounted prices
console.log("Discounted Prices:", discountedPrices);
// Task 5 - Filter Method for Product Availability

// Declare the inventory array with product quantities
let inventory = [5, 0, 12, 8, 0, 15];

// Use filter() to remove products with zero stock
let availableProducts = inventory.filter(quantity => quantity > 0);

// Log the filtered array
console.log("Available Products:", availableProducts);
// Task 6 - Revenue Calculation with Reduce Method

// Declare the sales array
let sales = [500, 300, 200, 400];

// Use reduce() to calculate total revenue
let totalRevenue = sales.reduce((accumulator, currentSale) => accumulator + currentSale, 0);

// Log the total revenue
console.log("Total Revenue:", totalRevenue);
// Task 7 - Customer Search with Find Method

// Declare the customers array
let customers = ["Alice", "Bob", "Charlie", "David"];

// Use find() to locate "Charlie"
let foundCustomer = customers.find(customer => customer === "Charlie");

// Log the result
console.log("Found Customer:", foundCustomer);
// Task 8 - Tax Calculation Function

// Function to calculate tax
function calculateTax(amount, taxRate) {
    return amount * taxRate;
}

// Example usage
let amount = 1000;
let taxRate = 0.08; // 8% tax
let tax = calculateTax(amount, taxRate);

// Log the calculated tax
console.log(`For an amount of $${amount}, the tax at ${taxRate * 100}% is $${tax.toFixed(2)}.`);
// Task 9 - Discount Application Function Expression

// Function expression to apply discount
const applyDiscount = function(price, discount) {
    return price - (price * discount);
};

// Example usage
let originalPrice = 200;
let discountRate = 0.15; // 15% discount
let discountedPrice = applyDiscount(originalPrice, discountRate);

// Log the result
console.log(`Original Price: $${originalPrice}`);
console.log(`Discounted Price: $${discountedPrice.toFixed(2)}`);
// Task 10 - Loyalty Points Arrow Function

// Arrow function to calculate loyalty points
const calculatePoints = purchaseAmount => Math.floor(purchaseAmount / 10);

// Example usage
let purchaseAmount = 125;
let points = calculatePoints(purchaseAmount);

// Log the result
console.log(`For a purchase of $${purchaseAmount}, you earn ${points} loyalty points.`);
