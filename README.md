# math2
def factorial(n):
    """
    Calculates the factorial of a number.
    """
    if n == 0:
        return 1
    return n * factorial(n - 1)

def is_prime(n):
    """
    Checks if a number is a prime number.
    """
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
if __name__ == "__main__":
    test_number = int(input("Enter a number: "))
    print(f"Factorial: {factorial(test_number)}")
    print(f"Is Prime: {is_prime(test_number)}")
