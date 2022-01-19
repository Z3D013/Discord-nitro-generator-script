# Discord-nitro-generator-script
script to my nitro generator i explained in: https://github.com/Z3D013/Discord-Nitro-Generator

.

import random

chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuwvxyz0123456789"

for i in range(100):
  first = ''.join((random.choice(chars) for i in range(16)))

  result = "https://discord.gift/" + first
  
  output = open("output.txt", "a")
  output.write(result + "\n")
