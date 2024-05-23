# OS-Project-Implementation

In this application, we have a Producer and multiple Consumers that work together to process a two-dimensional matrix of integers. Here’s a high-level overview of how the Producer and Consumers interact:

#Producer

Matrix Initialization: The Producer initializes a 100 x 100 matrix of integers.
Pointer Array Creation: It then creates an array of pointers, where each pointer points to the start of a row in the matrix.
Memory Address Production: The Producer stores the address of each row (a pointer to the first element of each row) into this array of pointers.


#Consumers

Pointer Array Access: Multiple Consumers access the array of pointers concurrently.
Row Processing: Each Consumer retrieves a pointer from the array, which corresponds to a specific row in the matrix.
Prime Calculation: The Consumer then iterates through the integers in that row, counts the number of prime numbers, and adds this count to a shared sum.
