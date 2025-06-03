sequence = "GATATATGCATATACTT"
pattern = "ATAT"


DNA = sequence.upper()
kmer = pattern.upper()
k = len(kmer)


output = []


for i in range(len(DNA) - k + 1):
    substring = DNA[i:i + k]
    if substring == kmer:
        output.append(str(i))


answer = ' '.join(output)
print(answer)# Pattern-matching-
