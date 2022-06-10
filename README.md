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
