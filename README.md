tickets = int(input("Введите количество билетов:"))
print("Укажите возраст каждого из посетителей")
price = 0
for i in range(tickets):
    age = int(input("Введите возраст:"))
    if age < 18:
        price += 0
    elif age >= 18 and age < 25:
        price += 990
    else:
        price += 1390

if tickets > 3:
    sale = 0.9
else:
    sale = 1
print("Итого к оплате, руб:", price * sale)
