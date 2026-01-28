number_of_terms = int(input("Enter the number of terms (greater than 2): "))

# initialize first and second terms
fibonacci_1 = 0
fibonacci_2 = 1

# initialize the next term (3rd term)
fibonacci_3 = fibonacci_1 + fibonacci_2

# print the first two terms
print("Fibonacci Series:")
print(fibonacci_1)
print(fibonacci_2)

# Using a while loop (closest to C do-while here, as Python has no native do-while)
i = 3
while True:
    print(fibonacci_3)
    fibonacci_1 = fibonacci_2
    fibonacci_2 = fibonacci_3
    fibonacci_3 = fibonacci_1 + fibonacci_2
    i += 1
    if i > number_of_terms:
        break
