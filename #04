sample = input("Sample Dataset : ")
sample = sample.split(" ")
n = int(sample[0])
k = int(sample[1])

x = [0]  # mature
y = [1]  # immature

for i in range(0, n - 1):
    x.append(x[-1] + y[-1])
    y.append(x[-2] * k)

print("Sample Output :", x[-1] + y[-1])

