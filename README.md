# Serial-Read
import serial
import time
import csv
import matplotlib
matplotlib.use("tkAgg")
import matplotlib.pyplot as plt
import numpy as np

ser = serial.Serial('COM6', 9600)

while True:
    data = ser.readline()
    print(data)
    
