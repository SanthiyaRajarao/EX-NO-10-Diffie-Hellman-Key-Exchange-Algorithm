# EX-NO-10-Diffie-Hellman-Key-Exchange-Algorithm

## AIM:
To Implement Diffie Hellman Key Exchange Algorithm 

NAME: SANTHIYA R

RED NO:212223230192
## Algorithm:

1. Diffie-Hellman Key Exchange is used for securely sharing a secret key between two parties over an insecure channel.

2. Initialization: Agree on a large prime number \( p \) and a primitive root \( g \) modulo \( p \) (both are public values).

3. Key Exchange Process: 
   - Each party selects a private key and calculates their public key using the formula \( g^{\text{private key}} \mod p \).
   - Each party then shares their public key with the other.

4. Secret Key Computation: 
   - Each party computes the shared secret key using the received public key and their own private key.

5. Security: The difficulty of computing discrete logarithms ensures that the shared key remains secure even if public values are intercepted.

## Program:
```
P = int(input("Enter Prime Number: "))
G = int(input("Enter Primitive Root: "))

a = int(input("Enter Private Key of SANTHIYA: "))
b = int(input("Enter Private Key of R: "))

A = (G ** a) % P
B = (G ** b) % P

secretA = (B ** a) % P
secretB = (A ** b) % P

print("Public Key of SANTHIYA:", A)
print("Public Key of R:", B)

print("Secret Key for SANTHIYA:", secretA)
print("Secret Key for R:", secretB)

if secretA == secretB:
    print("Secret key successfully established")
else:
    print("Keys do not match")

print("Program executed successfully")
```



## Output:
<img width="1919" height="794" alt="image" src="https://github.com/user-attachments/assets/0b8dcccf-a6cf-4905-89af-4d52736ff008" />



## Result:
  The program is executed successfully

