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
