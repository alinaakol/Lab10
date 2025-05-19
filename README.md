"""
Студент: Колісніченко
Створення файлу та запис першого питання
"""
try:
    # Відкриваємо файл у режимі запису (створиться новий)
    with open('programming_questions.txt', 'w', encoding='utf-8') as file:
        file.write("Прізвище: Колісніченко\n")
        file.write("Питання: Що означає функція print() в Python?\n")
        file.write("Відповідь:\n")
        file.write("Нове питання:\n")
    print("Файл успішно створено та дані вписано")
except IOError as e:
    print(f"Помилка роботи з файлом: {e}")
except Exception as e:
    print(f"Інша помилка: {e}")
