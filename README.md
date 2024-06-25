# python.
python program 2
# PYTHON-PROGRAM-7
program for CONVERSIONS OF INT TO ROMAN NUMBERS
def int_to_rom(num):
    val = [1000,500,100,50,10,5,1]
    sym = ["M","D","C","L","X","V","I"]
    roman_num = ''
    i = 0
    while num >0:
        for i in range(num // val[i]):
            roman_num += sym[i]
            num -= val[i]
        i += 1
    return roman_num
number = 75
print(f"The Roman numeral representation of {number} is {int_to_roman(number)}")
        
