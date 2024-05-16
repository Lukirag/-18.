sum_tickets = 0
tickets = int(input("Введите количество билетов: \n"))
for age in range (tickets):
    age = ("Введите возраст посетителя:: \n")
    if age < 18:
        sum_tickets += 0
    elif age >= 18 and age <= 25:
        sum_tickets += 990
    elif age > 25:
        sum_tickets += 1390
if sum_tickets == 0:
    print("Проходите, детки, на конференцию!")
else:
    print("Стоимость Ваших билетов:", "%.2f" % tickets, "руб.")
if tickets > 3:
    discount = sum_tickets / 100 * 10
    print("Скидка составляет:", "%.2f" % discount, "руб.")
    print("К оплате:", "%.2f" % (sum_tickets -discount), "руб.")
