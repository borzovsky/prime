def is_prime(number):
    if number < 2:
        return False

    for i in range(2, int(number ** 0.5) + 1):
        if number % i == 0:
            return False

    return True

# Prompt the user to enter a number
number = int(input("Enter a number: "))

# Check if the number is prime
if is_prime(number):
    print(number, "is a prime number.")
else:
    print(number, "is not a prime number.")
