# ggos-2022

## Загальний опис

Бла-бла-бла. Працює через Tor.

## Інструкція зі встановлення

* ### Встановлюємо Python якщо він не встановлений


  Встановлювальний файл Python для Windows можна знайти на [python.org](https://python.org) в розліді _Downloads_.

* ### Встановлюємо необхідні пакети для Python

  Виконуємо в консолі команду `pip install requests torpy`

* ### Завантажуємо та розпаковуємо ZIP-архів
 
  ZIP-архів знаходимо ось тут [github.com/ggos-2022/ggos-2022](https://github.com/ggos-2022/ggos-2022). Місце розпакування не важливе.

  ![image_2022-03-12_18-48-48](https://user-images.githubusercontent.com/100677310/158026955-5cad335e-b1e6-45fd-9a2f-6a764d8443eb.png)

* ### Список цільових сайтів вказуємо у файлі `target_sites.txt`

  Для сайту-цілі використувуємо окремий рядок. Зайвими пробілами на початку та у кінці рядка можна нехтувати. Зайвими порожніми рядками можна нехтувати. Для ігнорування сайту або для коментару можна на початку рядка використовувати символ `#`
  
  **Важливо**. Необхідно щоб на початку кожного сайту обов'язково було присутнє `http://` або `https://`
  
  Приклад файлу `target_sites.txt`:
  
  ![image](https://user-images.githubusercontent.com/100677310/158028048-fc1aa985-d6a5-4fd3-86cc-0bb3819f9dd1.png)


* ### Для старту програми запускаємо скрипт запуску `run.bat`

  ![image](https://user-images.githubusercontent.com/100677310/158027315-23baf215-5488-4f3d-9e84-f22c32c12010.png)

## Огляд

![image](https://user-images.githubusercontent.com/100677310/158029225-1873bfd4-eb82-49da-aa1e-db0dc855802d.png)


1-ша колонка з цифр — кількість успішних запитів.

2-га колонка — кількість останніх невдалих запитів підряд. Якщо раптом запит виконується успішно це число обнуляється. Щоб не робити запити на сайт, який вже напевне лежить, програма спить 2 в степені `це значення` секунд після невдалого запиту.

3-тя колонка — загальна кількість невдалих запитів.


У кінці вікна — технічні коментарі, можна ігнорувати.


У папці `logs` можна знайти логи до кожного сайту окремо.

