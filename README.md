# Project Description

for: Assignment-1 (UCS654) submitted by: Aryan Gupta  Roll no: 102103140   Group: 3COE5

Topsis-Aryan-102103140 is a Python library for dealing with Multiple Criteria Decision Making(MCDM) problems by using Technique for Order of Preference by Similarity to Ideal Solution(TOPSIS).

# Installation

`pip install Topsis-Aryan-102103145`

How to use it?

Enter csv filename followed by .csv extension, then enter the weights separated by commas, followed by the impacts with comma separated signs (+,-) and then the csv filename in which you want to store the result by .csv extension .

`Topsis sample.csv "1,1,1,2,2" "+,+,-,+,+" result.csv`


# Example

sample.csv

Fund Name,P1,P2,P3,P4,P5

M1,0.93,0.86,6.9,32.1,10.2

M2,0.73,0.53,5.5,36.9,10.92

M3,0.77,0.59,3.7,34.5,9.89

M4,0.61,0.37,3.6,54.7,14.82

M5,0.73,0.53,7,57.3,16.39

M6,0.67,0.45,6.3,46.4,13.46

M7,0.93,0.86,3.6,55.6,15.25 

M8,0.8,0.64,5.1,40.9,11.86

M8 0.81 0.66 3.7 35.9 10.27



weights vector = [ 1,1,3,2,2 ]

impacts vector = [ +,+,-,+,- ]


input

`Topsis sample.csv "1,1,3,2,2" "+,+,-,+,-" result.csv`



output

result.csv

Fund Name,P1,P2,P3,P4,P5,Topsis Score,Rank

M1,0.93,0.86,6.9,32.1,10.2,0.6568246813608912,3.0

M2,0.73,0.53,5.5,36.9,10.92,0.7507442242528632,2.0

M3,0.77,0.59,3.7,34.5,9.89,0.834669716472082,1.0

M4,0.61,0.37,3.6,54.7,14.82,0.38659050631435843,6.0

M5,0.73,0.53,7.0,57.3,16.39,0.20489354804132592,8.0

M6,0.67,0.45,6.3,46.4,13.46,0.47228704243057956,5.0

M7,0.93,0.86,3.6,55.6,15.25,0.25781450881467294,7.0

M8,0.8,0.64,5.1,40.9,11.86,0.6235072426142194,4.0



# Other Notes

1. The first column and first row are removed by the library before processing, in attempt to remove indices and headers. Make sure the csv follows the format as shown in sample.csv.

2. Make sure the csv does not contain categorical values

License

© 2024 Aryan Gupta

This repository is licensed under the MIT license.

See LICENSE for details.
