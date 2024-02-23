# Создаем словарь для преобразования чисел в слова
numbers = {
    '0': 'ноль',
    '1': 'один',
    '2': 'два',
    '3': 'три',
    '4': 'четыре',
    '5': 'пять',
    '6': 'шесть',
    '7': 'семь',
    '8': 'восемь',
    '9': 'девять'
}

# Считываем цифру, с которой должны начинаться четные числа
start_digit = input("Введите цифру (от 0 до 9): ")

# Главный цикл программы, эмулирующий чтение данных из файла
count = 0
file = open('D:\\example.txt','r',encoding='utf-8')

for string in file:
    string=''.join(i if i.isdigit() else ' ' for i in string).split()
    # Эмулируем чтение числа
    for number in string:

    # Проверяем, что число начинается с введенной цифры и является четным
        if number.startswith(start_digit) and int(number) % 2 == 0:
            count += 1
            if count % 5 == 0:
                print("Прописью:")
                for digit in number:
                    print(numbers[digit])
                print()
            else:
                print(number)
