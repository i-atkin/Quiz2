# Quiz2
Fibonacci sequence and the golden ration plot 

import numpy as np
import matplotlib.pyplot as plt

sequence = input("Fibonacci Sequence Number: ")

list = []
def fib(sequence):
    n1 = 0
    n2 = 1
    counter = 0

    while counter <= int(sequence):
        list.append(n1)
        n = n1 + n2
        n1 = n2
        n2 = n
        counter += 1

fib = fib(sequence)
seq = np.asarray(list)
print("Fibonacci Sequence to  " + str(sequence)+ " terms.")
print(seq)
