# oasis-task-1
import CsV 
import os

def load_data( filename):

data = []
*with open(filename, 'r') as file:
reader = csv.reader(file)
next(reader )T

for row in reader:

data. append(row)

return data

 def analyze_data(data):

species_counts = ()

for row in data:

species = row[4]


if species in species_counts:
species_counts [species| += 1

else:
species_counts[species] =1
print ("Species Counts: ")
for species, count in species_counts.items():
print(species, ":", count)

 filename = "Iris.csv"

 directory_path = "kaggle datasets download -d saurabh00007/1riscsy"

file_path = os.path.join(directory_path, filename)

data = load_data(file_path)
analyze_data(data)
