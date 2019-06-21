jout  =jin *s 
rout = rin + (k-1)*jin

# 1st layer - 7x7 stride =2

jout = 1*2 =2
rout = 1 + (7-1) *1 =6

# 2nd layer - Max pool 3x3 stride =2

jout = 2 * 2 = 4
rout = 6 +(3-1)*2 = 10

# 3rd layer - 3x3 stride =1

jout = 4 * 1 =4
rout = 10 + (3-1)*1 =12

# 4th layer - 3x3 stride =2

jout = 4*2 = 8
rout = 12 + (3-1)*2 = 16 

# 5th layer -Inception

-Max pool 3x3 stride =1
 
 jout = 8 * 1 = 8
 rout = 16 + 2 * 1 = 18

- 5x5 stride =1

jout = 8 * 1 = 8
rout = 16 + 4 * 1 = 20

- 3x3 stride =1 
 jout = 8 * 1 = 8 
 rout = 16 + 2 *1 = 18  

# 6th Layer - Inception

-Max pool 3x3 stride =1
 
 jout = 8 * 1 = 8
 rout = 16 + 2 * 1 = 18

- 5x5 stride =1

jout = 8 * 1 = 8
rout = 16 + 4 * 1 = 20

- 3x3 stride =1 
 jout = 8 * 1 = 8 
 rout = 16 + 2 *1 = 18  

# 7 th -Max pooling 3x3 ,stride =2

jout = 8 *2 =16

rout = 20 + (3-1) * 8 = 36

# 8 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 rout = 36 + 2 * 16 = 68

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 36 + 4 * 16= 100

- 3x3 stride =1 
 jout = 16 * 1 = 16 
 rout = 36 + 2 * 32 = 68  


# 9 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 rout = 100 + 2 * 16 = 132

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 100 + 4 * 16= 164

- 3x3 stride =1 
 jout = 16 * 1 = 16 
 rout = 100 + 2 * 16 = 132
 
 # 10 th layer - Inception 


-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 rout = 132 + 2 * 16 = 164

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 132 + 4 * 16= 196

- 3x3 stride =1 
 jout = 16 * 1 = 16 
 out = 132 + 2 * 16 = 164
 
 # 11 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 rout = 196 + 2 * 16 = 228

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 196 + 4 * 16= 260

- 3x3 stride =1 
 jout = 16 * 1 = 16 
 out = 196 + 2 * 16 = 228
 
 # 12 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 rout = 260 + 2 * 16 = 292

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 260 + 4 * 16= 324

- 3x3 stride =1 
  jout = 16 * 1 = 16
 rout = 260 + 2 * 16 = 292
 
# 13th layer 3x3 ,Stride =2

jout = 16 * 2 = 32
rout = 324 + 4 * 16= 388

# 14 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 32 * 1 = 16
 rout = 388 + 2 * 16 = 420

- 5x5 stride =1

jout = 32 * 1 = 32
rout = 388 + 4 * 16= 452

- 3x3 stride =1 
  jout = 32 * 1 = 32
 rout = 388 + 2 * 16 = 420
 
 # 15 th layer - Inception  (Taking Max receptive field from previous layers)

-Max pool 3x3 stride =1
 
 jout = 32 * 1 = 32
 rout = 452 + 2 * 32 = 516

- 5x5 stride =1

jout = 32 * 1 = 32
rout = 452 + 4 * 32= 580

- 3x3 stride =1 
  jout = 32 * 1 = 32
 rout = 452 + 2 * 32 = 516
 
 
