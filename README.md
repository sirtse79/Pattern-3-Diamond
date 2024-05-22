# Pattern-3-Diamond
It works too

num = int(input())
row = 0
even_value = 1

print("   r")
print("   o")
print("   w")

for i in range(1, num + 1, 2):
    row += 1
    needed_free_space = str(row)
    space = len(needed_free_space)
    space_str = (3 - space) * " "
    print(space_str, row, end ='')
    print((num - i) // 2 * " ", i * "*", end = (num - i) // 2 * " ")
    print(f" i = {i} | num - i = {num - i} | (num - i) // 2 = {(num - i) // 2}")

if num % 2 == 1:
    even_value = 2

for i in range(num - even_value, 0, -2):
    row +=1
    needed_free_space = str(row)
    space = len(needed_free_space)
    space_str = (3 - space) * " "
    print(space_str, row, end ='')
    print((num - i) // 2 * " ", i * "*", end = (num - i) // 2 * " ")
    print(f" i = {i} | num - i = {num - i} | (num - i) // 2 = {(num - i) // 2}")
