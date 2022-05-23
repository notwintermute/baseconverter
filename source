inp = 245724578  # input
base = 16  # target base
col = []  # where the number will be stored

# Divide the decimal number by the radix of the target base
# The remainder from step 1 becomes the value for the current column.
# Use the quotient (answer) from step 1 as the decimal value to calculate the next column.
# Return to step 1 and repeat until the quotient is zero.
alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"

dec = inp
while dec > 0:
    dec, rem = divmod(dec, base)
    if rem >= 10: # if the number cant be represented with 0-9 replace it with alphabet characters
        col.insert(0, alphabet[rem-10])
    else:
        col.insert(0, str(rem))

# prints result
print(f"{inp} in base {base} is", ''.join(col))
