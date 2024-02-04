#This program helps the seller determine whether a buyer needs a discount and calculates it. 
price = input('Enter the price: ')
discount_percent = int(input('Enter the discount offered: ')) 

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        return discount_percent*0.2
    else:
        return 0
    
new_price = price-calculate_discount(price, discount_percent)
print(new_price)
