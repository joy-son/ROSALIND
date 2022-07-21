from operator import itemgetter, attrgetter

sample = input("File name : ")
sample = sample + ".txt"
header = ""
d_fasta = {}
GC = 0
output = []

r_sample = open(sample, "r")
for line in r_sample:
    line = line.strip()

    if line.startswith(">"):
        header = line[1:]
        d_fasta[header] = ""
    else:
        d_fasta[header] += line

for h, s in d_fasta.items():
    GC = (s.count("G") + s.count("C")) / len(s) * 100
    output.append([h, s, GC])

output = sorted(output, key=itemgetter(2), reverse=True)

print("Sample Output :")
print(output[0][0])
print(round(output[0][2], 6))

