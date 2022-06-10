## Sieve_of_Eratosthenes
# n = input number 
# m = prime number 

def is_prime(n): 
    """Test if a number is a prime"""
    for i in range(2, int(n ** 0.5)+1):
        if n % i == 0:
            return False
    return True
    
def Sieve_of_Eratosthenes(n):
    """Produce the sieve of Eratosthenes that lists all the 
    prime numbers less than or equal to n
    """
    
    global is_prime
    global m
    
    is_prime = is_prime
    m = n
    l = [True] * (m - 1)  
    for i in range(2, m): 
        if l[i]: 
            continue
        for j in range(i*i, m, i): 
            l[j] = False
    return l        
        
# test driver 

for n in range(10):
    for i in S
## This function  is
# called by the for loop and checks whether each number is a prime or
# not.
# If a sieve exists, return the one with the smallest running time.
# Otherwise, create a new one.
# For each number in sieve_data, print the first time it appears in
# the sieve.
"""
if __name__ == "__main__":
import sys
import time
import math
sys.stdout.write("Start the Python console to run the examples.")
sys.stdout.flush()
sys.stdout.write("Usage:")
for i in range(4, 2):
sys.stdout.write("Python example #{"i}
")
start_sieve_data(1000, sieve_of_eratosthenes("123456789"))
sys.stdout.write("End the Python console to run the examples.")
sys.stdout.flush()
print("Running time:", time.clock(), "seconds.")
def sieve_of_eratosthenes(n):
# Write a list that contains all the multiples of all the prime numbers 
# less than or equal to n.
# Sort the list so the first appearance of each prime number appears at 
# the beginning.
# For each number in sieve_data, print the first time it appears in
# the sieve.

# Create a list of prime numbers 
primes = []

# Find all the primes
for i in range(2, math.sqrt(n)+1):
    if is_prime(i):
        primes.append(i)
    if n % i == 0:sieve_data.append(i)
print("Primes less than or equal to", n)
# Display the primes less than n
for i in range(2, int(n ** 0.5)+1):
    if is_prime(i):
        if n % i == 0:
            print("\\n" + str(i) + ":", end=' ')
print("\n-----------------------------------------------------")

# If there are no primes less than n, print "Impossible"
# Create a list that contains all the multiples of all the primes
# less than n.
multiples = []

for i in range(2, n):
    for j in range(2, i+1):
        if i % j == 0:
               multiples.append(i)
            for p in primes:
                if i % p == 0:
                    multiples.append(p)

# Sort the list so the multiples of the smallest prime appear first.
multiples = sorted(multiples)

# For each multiple of a prime, print the first time it appears in the sieve
for i in range(2, len(multiples)):
    if (i in sieve_data):
        if (multiples[i] == sieve_data[i]):
            print("\\n" + str(i) + ":", end=' ')
    else:
        print("Impossible")
print("\n-----------------------------------------------------")
sys.stdout.write("Finished generating and sorting the sieve of 
Eratosthenes data in ", time.clock(), "seconds.")
sys.stdout.write("Run the Python code to see the sieve.")
start_sieve_data(1000, sieve_of_eratosthenes("123456789"))
sys.stdout.write("End the Python console to run the examples.")
sys.stdout.flush()
print("Running time:", time.clock(), "seconds.")
Running time: 2.531 seconds
Start the Python console to run the examples.
A prime number is a number greater than 1 that is only divisible by 1 and itself.
The Sieve of Eratosthenes is the best known algorithm to find prime numbers.
It was described by the Greek mathematician Archimedes in 212 BC.
It does not consider the prime factors of a number, but lists all the multiples of all the prime numbers less than or equal to n.
For example, we can find all the multiples of 3:
1, 3, 6, 9, 15,
