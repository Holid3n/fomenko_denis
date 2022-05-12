# Условия: if, else, elif. Блоки, отступы
![image](https://user-images.githubusercontent.com/97594334/168150571-e919b4f1-0930-44ff-a6b1-ee123d96c15b.png)
![image](https://user-images.githubusercontent.com/97594334/168150616-d8503fab-10c7-4525-b83e-5cf51aeccbe7.png)
# Первый код
![image](https://user-images.githubusercontent.com/97594334/168150648-334c65fc-0e08-4841-9a57-8496f1fe53c2.png)
a = int(input()) <br>
b = int(input()) <br>
c = int(input()) <br>
if b >= c >= a: <br>
    print('Это нормально') <br>
elif c >= b: <br> 
    print('Пересып') <br>
elif c <= a: <br>
    print('Недосып') <br>
# Второй код
![image](https://user-images.githubusercontent.com/97594334/168150706-cf664cd1-96d9-4556-9663-6afb6c30faf7.png)
a = int(input()) <br>
if a % 4 == 0 and a % 100 != 0 or a % 400 == 0: <br>
    print("Високосный") <br>
else: <br>
    print("Обычный") <br
