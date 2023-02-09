#  Звіт до лабораторної роботи №1
##  Тема: Робота з бібліотекою numpy
###  Мета роботи: Навчіться працювати з бібліотекою numpy.
---
## **Виконання роботи** 

***- Результати виконання завдань:***


###  Встановлення бібліотеки `NumPy`
Для початку встановлюю бібліотеку `NumPy` . Ця команда виконується в командній строчці (потрібно мати встановлений Python та `pip` ).
```баш
pip встановити numpy
```
Як видно на скріні нижче, бібліотека `numpy` вже інстальована. Система пропонує оновити версію `pip` з версій 22.2.2 до 22.3.1. Оновімо `pip` .

![ текст альтернативи ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/2.jpg "Оновлення `pip`")

Дана бібліотека дозволяє працювати з іншими типами даних ("Numeric Python" - числовими), спрощуючи їх використання, визначене в класичному Python, додає можливість працювати з векторами та матрицями.
Для роботи з бібліотекою будемо працювати інтерактивно в Jupytere Notebook.

Для цього:
- створила файл `numpy.ipynb` ;
- всі файли розмістила в репозиторії Github.

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/1.jpg "`numpy.ipynb`")

_______
1. Заданий список температур:
    ```пітон
        імпортувати numpy як np
        температура = [ 20.1 , 20.1 , 20.2 , 20.4 ]
        друк (температура)
    ```
## **Робота з простими листами:** 


![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/3.jpg "Результат обчислень")

### **~ДОМАШНЄ ЗАВДАННЯ~** 

Таким чином, множення неуспішне((( В результаті отримано новий список температур `t1` , кількість елементів якого збільшена в 5 разів порівняно з початковим `t1=temperature*5`

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/4.jpg "Результат обчислень")


### **~ДОМАШНЄ ЗАВДАННЯ~** 

Отже, множення успішне! У результаті отримано новий список температур `t1` , кожен елемент якого помножений на 5 та збільшений на 30 `t1=temperature*5`

## **Робота з листами в бібліотеці `numpy` :** 
![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/5.jpg "Результат обчислень")
________

## **Вектори, створення та робота з ними** 

```пітон
l1 = [ 1 , 2 , 3 , 4 , 5 ]
l2 = [ 6 , 7 , 8 , 9 , 10 ]
l3 = [ 11 , 12 , 13 , 14 , 15 ]
vector_1 = np.array(l1)
вектор_2 = np.array([l1, l2])
vector_3 = np.array([l1, l2, l3])
vector_4 = np.array([[l1, l2, l3], [l1, l2, l3], [l1, l2, l3], [l1, l2, l3]])
print ( f " Це список: { l1 } \n\n Масив numpy `vector_1`: { vector_1 } \n\n Масив numpy `vector_2`: \n { vector_2 } \n\n Масив numpy `vector_3`: \ n { vector_3 } \n\n Масив numpy `vector_4`: \n { vector_4 } " )      
t1 = вектор_1 * 7
t2 = вектор_2 * 7
t4 = вектор_4 * 7
print ( f " \n Результат множення елементів масиву 'vector_1' на 7: { t1 } , \n Результат множення масиву 'vector_2' на 7: { t2 } , \n Результат множення масиву 'vector_4' на 7: { t4 } " )
```

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/6.jpg "Результат обчислень")
![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/7.jpg "Результат обчислень")
![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/8.jpg "Результат обчислень")

## **Метод arange - генерує послідовність чисел з певним кроком у заданому інтервалі** 

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_9.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_10.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_11.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_12.jpg "Результати")


## **Метод linspace - генерує задану кількість чисел у певній області, 50 чисел за замовчуванням** 

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_13.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_14.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_15.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_16.jpg "Результати")


## **Типи масивів/векторів, багатовимірні масиви, розуміння вимірів** 

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_17.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_18.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_19.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_20.jpg "Результати")

## **Індексація та нарізка** 

***Індексування*** - використання для доступу до елементів масиву.

*** Slicing*** - використовується для доступу до кількох елементів зображення.

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_21.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_22.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_23.jpg "Результати")


Для доступу до кількох елементів вибору Slicing.

Принцип доступу до елементів   `S[start:stop:step]` . Елемент `stop` не включається у вивід.

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_24.jpg "Результати")

Такий самий принцип нарізку можна використовувати для багатовимірних масивів.

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_25.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_26.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_27.jpg "Результати")

Нарізка дозволяє брати не тільки наступні, але значення із заданим кроком.

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_28.jpg "Результати")

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_29.jpg "Результати")

Можна вибрати вибірку елементів за умовами

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_30.jpg "Результати")

## **Функції для створення матриці: одиниці, нулі, ідентичність, око, пусто** 

![ альтернативний текст ](https://github.com/KhrystynaKlym/KN320_Digit_Methods/raw/main/Lab_01/Screenshots/Screenshot_31.jpg "Результати")


    

            
        
______
______
_____
  
### ***Висновок:*** 

- втсановив бібліотеку `numpy`  : heavy_check_mark :
- навчився створювати вектори та працювати з ними : heavy_check_mark :
- працює з методами `arange` та `linspace`  : heavy_check_mark :
- ознайомився із типами масивів/векторів : heavy_check_mark :
- ознайомився з багатовимірними масивами та зрозуміла їхню вимірність : heavy_check_mark :
- працює із `Indexing` та `Slicing`  : heavy_check_mark :
- ознайомився з функціями для створення матриці: `ones` , `zeros` , `identity` , `eye` , `empty`  : heavy_check_mark :
- дав відповіді на поставлені завдання : heavy_check_mark :
- роботу оформив. Все гуд : heavy_check_mark :
- все виконано, всі завдання виконані : heavy_check_mark :
- завдяки Вашому детальному поясненню жодної складності не виникло : ok_hand :
- так, подобається; це зручний формат здачі роботи : thumbsup :
- поки що побажань немає, все ГУД : smiley :