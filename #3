sample = input("Sample Dataset : ")
output = []
d_nuc = {"A": "T", "C": "G", "T": "A", "G": "C"}

for i in range(len(sample)):
    if sample[i] in d_nuc.keys():
        output.append(sample[i].replace(sample[i], d_nuc[sample[i]]))

output = "".join(output)
print("Sample Output :", output[::-1])
