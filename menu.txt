import csv
csv_file = open('C:/Users/Surbhi/Desktop/menu.csv')
csv_reader = csv.reader(csv_file, delimiter = ',')
date = int(input("Enter date from 16 to 31 of which menu you want to see: "))
for row in csv_reader:
   d = []
   for i in range(1,17):
      d.append(row[i])
   print(d[date-16])
csv_file.close()
