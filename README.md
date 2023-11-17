COLUMNAR TRANSPOSITION CIPHER
Involves writing plaintext in rows and then reading ciphertext off in columns.

ENCRYPTION
We first pick a keyword for our encryption. We write the plaintext out in a grid where the number of columns is the number of the letters in the keyword. We then title each column with the respective letter from the keyword. We take the letters in the key word in alphabetical order, and read down the columns in this order. If a letter is repeated, we do the one that appears first, then the next and so on.

As an example, let’s encrypt the message “The tomato is a plant in the nightshade family” using the keyword tomato. We get the grid given below

T
O
M
A
T
O
5
3
2
1
6
4
T
H
E
T
O
M
A
T
O
I
S
A
P
L
A
N
T
I
N
T
H
E
N
I
G
H
T
S
H
A
D
E
F
A
M
I
L
Y
X
X
X
X

We have written the keyword above the grid of the plaintext, and also the numbers telling us which order to read the columns in. Notice that the first “O” is 3 and the second “O” is 4, and the same thing for the two “Ts”.
Starting with the column headed by “A” our ciphertext beigns “TINESAX” from this column. We move on to the column headed by “M” and so on through the letters of the keyword in alphabetical order to get the ciphertext “TINESAX / EOAHTFX / HTLTHEY / MAIIAIX / TAPNGDL / OSTNHMX” (where the / tells you where a new column starts). The final ciphertext is thus “TINES AXEOA HTFXH TLTHE YMAII AIXTA PNGDL OSTNHM.”

DECRYPTION
The encryption process is significantly easier if nulls have been used to pad out the message in the encryption process. Below we shall talk how to go about decrypting a message in both scenarios.

Firstly, if nulls have been used, then you start by writing out the keyword and the alphabetical order order of the letters of the keyword. You must then divide the length of the ciphertext by the length of the keyword. The answer to this is the number of rows you need to add to the grid. You then write the ciphertext down the first column until you reach the last row. The next letter becomes the first letter in the second column (by the alphabetical order of the keyword), and so on.

As an example, we shall decrypt the ciphertext “ARESA SXOST HEYLO IIAIE XPENG DLLTA HTFAX TENHM WX” given the keyword potato. We start by writing out the keyword and the order of the letters.There are 42 letters in the ciphetext, and the keyword has six letters so we need 42 / 6  = 7 rows.

                     
P
O
T
A
T
O
4
2
5
1
6
3











































Now we start by filling in the columns in the order given by the alphabetical order of the keyword, starting with the column headed by “A”. After the column is entered we have the grid shown  below.
We continue to add columns in the order specified by the keyword.

P
O
T
A
T
O
4
2
5
1
6
3



A





R





E





S





A





S





X



P
O
T
A
T
O
4
2
5
1
6
3

O

A



S

R



T

E



H

S



E

A



Y

S



L

X



After inserting the second columns

P
O
T
A
T
O
4
2
5
1
6
3

O

A

O

S

R

I

T

E

I

H

S

A

E

A

I

Y

S

E

L

X

X

After inserting the third column

P
O
T
A
T
O
4
2
5
1
6
3
P
O
T
A
T
O
E
S
A
R
E
I
N
T
H
E
N
I
G
H
T
S
H
A
D
E
F
A
M
I
L
Y
A
S
W
E
L
L
X
X
X
X

After completely reconstructing  the grid.

Now we read off the plaintext row at a time to get  “potatoes are in the nightshade family as well” 

When no null have been used we have to do a slightly different calculation. We divide the length of the ciphertext by the length of the keyword, but this is likely to not be a whole number. If this is the case, then we round the answer up to the next whole number, we then multiply this number by the length of the keyword, to find out how many boxes there are in total in the grid. Finally, we take the length of the ciphertext away from this answer. This number (which would be less than the length of the key) is how many nulls there would have been if used, so we need to black out these last few boxes, so we don’t put letters in them whilst decrypting.
To decrypt the ciphertext “ARESA SOSTH EYLOI IAIEP ENGDL LTAHT FATEN HMW.” we start similarly to above, by heading the columns with the keyword potato. This time, to find how may rows we need, we do 38 / 6 =  6.3333. We round this up to the next number, which is 7, so we need 7 rows. When we multiply 6 * 7  we get 42, and 42 – 38 = 4. Hence we need 4 placeholders in the last row. 
To decrypt the ciphertext “ARESA SOSTH EYLOI IAIEP ENGDL LTAHT FATEN HMW.” we start similarly to above, by heading the columns with the keyword potato. This time, to find how may rows we need, we do 38 / 6 =  6.3333. We round this up to the next number, which is 7, so we need 7 rows. When we multiply 6 * 7  we get 42, and 42 – 38 = 4. Hence we need 4 placeholders in the last row. 

              
