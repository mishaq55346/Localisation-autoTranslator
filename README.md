# Localisation-autoTranslator
---
Ну во-первых ссылочка на [автора](https://vk.com/sobol503)
---
Программа переводит файлы локализации игры **Hearts of Iron 4** с английского на русский и наоборот.

### Как пользоваться:
1. Закидываем файлы локализации на английском/русском языке в папку **"input"**(в папке уже есть пример файлов локализации).
2. Запускаем файл **"start.bat"**, ждем окончания работы программы, закрываем консоль и открываем папку **"output"**.
(скорость перевода зависит от количества строк в файле и скорости интернет-соединения)

### Как работает программа:
1. Программа берет файлы локализации из папки "input", удаляет все переменные(типа $var$, §%var§! и [THIS.var]) и убирает форматирование(цвета), оставляя текст в форматировании нетронутым.
2. Отправляет отредактированный текст по строкам API Yandex Translator
3. Генерирует файл локализации в папке output, сохраняя id и вставляя внутрь кавычек переведенный текст
4. Если что-то идет не так, создает файл error.txt с описанием ошибки 

### Если открыли папку "output" и не видите ничего, пройдитесь по пунктам:
1. Проверьте, установлена ли у вас **Java**
2. Проверьте, существуют ли папки "bin", "input" и "output" и нет ли ошибок в их названии
3. Проверьте, не пустая ли папка bin(должна иметь внутри текстовой файл с ключом и саму программу)
4. Удостоверьтесь, что файл "Translator.jar" находится в той же директории, что и папки "input" и "output"
5. Локализация должны быть написаны правильно(пример локализации можно увидеть в ваниле)
6. Файлы в папке "input" должны быть с расширением ".yml"
---
Если программа все равно не работает, пишите в лс(желательно с вложенным файлом "error.txt")^
