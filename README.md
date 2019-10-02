# Hello-World
Bioinformatics
# caculate GC content from file turtledemo.chaos import g

gene = open("lamma.txt", "r")
G = 0;
A = 0;
C = 0;
T = 0;
# 'skip the first line'
gene.readline()
for line in gene:
    line = line.upper()
    for char in line:
        if char == "G":
            G += 1
        if char == "A":
            A += 1
        if char == "C":
            C += 1
        if char == "T":
            T += 1
print(" number of g = " + str(G))
print(" number of c = " + str(C))
print(" number of t = " + str(T))
print(" number of a = " + str(A))
GC_percnt = (G + C+0.) / (A + T + C + G+0.) *100
print("gc_content = " + str(GC_percnt))
