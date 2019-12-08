# Python
import matplotlib.pyplot as plt
from matplotlib import pyplot as pt
import numpy as np
import seaborn as sbr


def Sine_Wave(blink=2):
    print("Sine Wave")
    start = int(input("enter the starting value"))
    end = int(input("enter the ending value"))
    breaks = int(input("enter the break points..."))
    x = np.linspace(start, end, breaks)
    a = int(input("enter the number for sine function"))
    for i in range(0, a):
        pt.plot(x, np.sin(x + i * 4) * (5 - i) * blink)
        plt.xlabel('x', fontweight='bold', fontsize=12)
        plt.ylabel(r'$\sin x$', fontweight='bold', fontsize=12)
        plt.title('Wave', fontweight='bold', fontsize=14)
        plt.grid(True)


sbr.set()
Sine_Wave()
pt.show()
print(" ")
print("Cosine Wave")


def cosine_Wave(blink=2):
    start = int(input("enter the starting value"))
    end = int(input("enter the ending value"))
    breaks = int(input("enter the break points..."))
    x = np.linspace(start, end, breaks)
    a = int(input("enter the number for cosine function"))
    for i in range(0, a):
        pt.plot(x, np.cos(x + i * 4) * (5 - i) * blink)
        plt.xlabel('x', fontweight='bold', fontsize=12)
        plt.ylabel(r'$\cosine x$', fontweight='bold', fontsize=12)
        plt.title('Wave', fontweight='bold', fontsize=14)
        plt.grid(True)


sbr.set()
cosine_Wave()
pt.show()
print(" ")
print("tan Wave")


def tan_wave(blink=2):
    start = int(input("enter the starting value"))
    end = int(input("enter the ending value"))
    breaks = int(input("enter the break points..."))
    x = np.linspace(start, end, breaks)
    a = int(input("enter the number for tan function"))
    for i in range(0, a):
        pt.plot(x, np.tan(x + i * 4) * (5 - i) * blink)
        plt.xlabel('x', fontweight='bold', fontsize=12)
        plt.ylabel(r'$\tan x$', fontweight='bold', fontsize=12)
        plt.title('Wave', fontweight='bold', fontsize=14)
        plt.grid(True)


sbr.set()
tan_wave()
pt.show()
