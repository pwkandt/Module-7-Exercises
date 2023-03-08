fileName = input('Enter file name: ')

try:
    fileHandle = open(fileName)
except:
    print('File cannot be opened:', fileName)
    quit()

count = 0
total = 0
for line in fileHandle:
    if line.startswith('X-DSPAM-Confidence:'):
        fLine = float(line[20:27])
        count = count + 1
        total = total + fLine

finalTotal = total / count
print('Average spam confidence:',finalTotal)
