#Combining SNTC Controllers CSV Files into one CSV File.

import os

## This is the path where you want to search the csv file r'D:\Python' and combine any csv file from this directory
dirs = [r'D:\Python']  

#out file combine csv file 'combine.csv'
outfile = open(r'D:\Python\combine.csv', 'wb')
for dir in dirs:
    for pathinfo in os.walk(dir):
        for file in pathinfo[2]:
            if file[-4:]!='.csv' or file=='combine.csv': continue   # any file .csv extension extracting while excluding combine.csv file
            filepath = pathinfo[0] + '\\' + file
            print(filepath)
            with open(filepath, 'rb') as f: outfile.write(f.read())               
outfile.close()   


