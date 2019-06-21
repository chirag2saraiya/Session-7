jout  =jin *s 
rout = rin + (k-1)*jin
### Assumption : 
1> Taking Max receptive field from previous layers  in Inseption
2> As per diagram shown on page 7, Maxpool in Inseption is 3x3 and Stride = 1 ,so took that value
3> Also considered calculations for Receptive field and Jump

# 1st layer - 7x7 stride = 2

jout = 1*2 =2

rout = 1 + (7-1) *1 =6

# 2nd layer - Max pool 3x3 stride =2

jout = 2 * 2 = 4

rout = 6 +(3-1)*2 = 10

# 3rd layer - 3x3 stride = 1

jout = 4 * 1 = 4

rout = 10 + (3-1)*1 =12

# 4th layer - 3x3 stride = 2

jout = 4*2 = 8

rout = 12 + (3-1)*2 = 16 

# 5th layer -Inception

-Max pool 3x3 stride =1
 
jout = 8 * 1 = 8
 
rout = 16 + 2 * 1 = 18

-5x5 stride =1

jout = 8 * 1 = 8

rout = 16 + 4 * 1 = 20

-3x3 stride =1 

 jout = 8 * 1 = 8
 
 rout = 16 + 2 *1 = 18  

# 6th Layer - Inception

-Max pool 3x3 stride =1
 
 jout = 8 * 1 = 8
 
 rout = 20 + 2 * 1 = 22

- 5x5 stride =1

jout = 8 * 1 = 8

rout = 20 + 4 * 1 = 24

- 3x3 stride = 1 

 jout = 8 * 1 = 8
 
 rout = 20 + 2 * 1 = 22

# 7 th -Max pooling 3x3 ,stride =2

jout = 8 * 2 =16

rout = 24 + (3-1) * 8 = 40

# 8 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 
 rout = 40 + 2 * 16 = 72

- 5x5 stride =1

jout = 16 * 1 = 16

rout = 40 + 4 * 16= 104

- 3x3 stride =1 

 jout = 16 * 1 = 16
 
 rout = 40 + 2 * 16 = 72 


# 9 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 
 rout = 104 + 2 * 16 = 136

- 5x5 stride =1

jout = 16 * 1 = 16
rout = 100 + 4 * 16= 164

- 3x3 stride =1 

jout = 16 * 1 = 16
 
rout = 104 + 2 * 16 = 136
 
 # 10 th layer - Inception 


-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 
 rout = 164 + 2 * 16 = 196

- 5x5 stride =1

jout = 16 * 1 = 16

rout = 164 + 4 * 16= 228

- 3x3 stride =1 

 jout = 16 * 1 = 16
 
 rout = 164 + 2 * 16 = 196
 
 # 11 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 
 rout = 228 + 2 * 16 = 260

- 5x5 stride =1

jout = 16 * 1 = 16

rout = 228 + 4 * 16= 292

- 3x3 stride =1 

 jout = 16 * 1 = 16 
 
 rout = 228 + 2 * 16 = 260
 
 # 12 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 16 * 1 = 16
 
 rout = 292 + 2 * 16 = 324

- 5x5 stride =1

jout = 16 * 1 = 16

rout = 292 + 4 * 16= 356

- 3x3 stride = 1

 jout = 16 * 1 = 16
 
 rout = 292 + 2 * 16 = 324
 
# 13th layer 3x3 ,Stride =2

jout = 16 * 2 = 32

rout = 356 + 4 * 16= 420

# 14 th layer - Inception 

-Max pool 3x3 stride =1
 
 jout = 32 * 1 = 16
 
 rout = 420 + 2 * 16 = 452

- 5x5 stride =1

jout = 32 * 1 = 32

rout = 420 + 4 * 16= 484

- 3x3 stride =1 

 jout = 32 * 1 = 16
 
 rout = 420 + 2 * 16 = 452
 
 # 15 th layer - Inception  

-Max pool 3x3 stride =1
 
 jout = 32 * 1 = 32
 
 rout = 484 + 2 * 32 = 548

- 5x5 stride =1

jout = 32 * 1 = 32

rout = 548 + 4 * 32= 676

- 3x3 stride =1 

jout = 32 * 1 = 32
 
rout = 484 + 2 * 32 = 548
 
 
