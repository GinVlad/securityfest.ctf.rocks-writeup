Use uncompyle2 to decompile flux.pyc
Then decode it in python:
`flag = [67,
 78,
 70,
 70,
 127,
 117,
 95,
 115,
 64,
 70,
 100,
 120,
 83,
 100,
 96,
 80,
 99,
 65,
 38,
 112,
 39,
 104]
f = ""
for x in range(len(flag)):
	f += chr(flag[x] ^ x )
print f`
