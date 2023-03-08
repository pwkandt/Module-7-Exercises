fileName = input('Enter file name: ')

if fileName == 'na na boo boo':
    print("NA NA BOO BOO TO YOU - You have been punk'd!")
    quit()

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
