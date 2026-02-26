import tkinter as tk

# Создаем главное окно
root = tk.Tk()
root.title("Веб-индексатор")
root.geometry("600x400")

# Заголовок
label = tk.Label(root, text="Веб-индексатор", font=("Arial", 16))
label.pack(pady=10)

# Поле для ввода URL
url_label = tk.Label(root, text="Введите URL сайта:")
url_label.pack()

url_entry = tk.Entry(root, width=50)
url_entry.pack(pady=5)
url_entry.insert(0, "https://example.com")

# Кнопка
button = tk.Button(root, text="Начать индексацию", bg="green", fg="white")
button.pack(pady=10)

# Текстовое поле для результатов
result_text = tk.Text(root, height=10, width=70)
result_text.pack(pady=10)

# Запуск приложения
root.mainloop()
