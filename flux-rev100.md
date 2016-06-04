Use uncompyle2 to decompile flux.pyc <br />
Then decode it in python: <br />
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
 104]` <br />
`f = ""` <br />
`for x in range(len(flag)): f += chr(flag[x] ^ x )` <br />
`print f` <br />
