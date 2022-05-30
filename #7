#!/usr/bin/env python
# k = number of homozygous dominant organisms
# m = number of heterozygous organisms
# n = number of homozygous recessive organisms

sample = input("Sample Dataset : ")
k = int(sample.split(" ")[0])
m = int(sample.split(" ")[1])
n = int(sample.split(" ")[2])

from scipy.special import comb


def cProbability(k, m, n):
    # Calculate total number of organisms in the population:
    total = k + m + n
    # Calculate the number of comb that could be made (valid or not):
    totalC = comb(total, 2)
    # Calculate the number of comb that have a dominant allele therefore are valid:
    validC = comb(k, 2) + k * m + k * n + 0.5 * m * n + 0.75 * comb(m, 2)
    probability = validC / totalC
    return probability


print(cProbability(k, m, n))
