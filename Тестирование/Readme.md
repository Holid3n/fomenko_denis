основы тестирования

Тестирование сейчас - проверка соответствия между реальным поведением программы и ее ожидаемым поведением на конечном наборе текстов, выбранном определенным образом.

Тестирование ПО может быть статическим и динамическим Статическое - без исполнения программного продукта Динамическое - во время выполнения программы

Определение тестирование:

Объект тестирования: Компонент или система, которые что-то там...

Дефект - изъяне в компоненте или системе, который может привести компонент или систему к невозможости выполнить требуемую функцию.

Верификация доказанное объективными результатами исследования подтверждение того,

Валидация определение соответствия разрабатываемого ПО ожиданиями и потребности пользователей.
# Первый код

using NUnit.Framework;
using Kalkulator;

namespace TestManipulator
{
    

    public class Tests
    {
        int num;

        [SetUp]
        public void Setup()
        {
        }

        [Test]
        public void TestSum()
        {
            // Arrange
            int a = 6;
            int b = 2;

            int actual = Class1.Sum(a, b);
            int expected = 8;
            Assert.AreEqual(expected, actual);
            /*
            if(num == 0)
            {
                int actual = Class1.Sum(a, b);
                int expected = 8;
                Assert.AreEqual(expected, actual);
            }
            else if(num == 1)
            {
                int actual = Class1.Raz(a, b);
                int expected = 4;
                Assert.AreEqual(expected, actual);
            }
            else if(num == 2)
            {
                int actual = Class1.Pro(a, b);
                int expected = 12;
                Assert.AreEqual(expected, actual);
            }
            else if(num == 3)
            {
                int actual = Class1.Chas(a, b);
                int expected = 3;
                Assert.AreEqual(expected, actual);
            }
            */
            // Act        
            // вызов функции
            // задать переменную: тип данных и название

            // Assert
            // Assert.AreEqual(expected, actual);
        }

        [Test]
        public void TestRaz()
        {
            int a = 6;
            int b = 2;

            int actual = Class1.Raz(a, b);
            int expected = 4;
            Assert.AreEqual(expected, actual);
        }

        [Test]
        public void TestPro()
        {
            int a = 6;
            int b = 2;

            int actual = Class1.Pro(a, b);
            int expected = 12;
            Assert.AreEqual(expected, actual);
        }

        [Test]
        public void TestChas()
        {
            int a = 6;
            int b = 2;

            int actual = Class1.Chas(a, b);
            int expected = 3;
            Assert.AreEqual(expected, actual);
        }
    }
}


# Второй код

using System;

namespace Kalkulator
{
    public class Class1
    {
        // создание функции сложения
        // модифактор доступа ()имя функции (данные) {}
        public static int Sum(int a, int b)
        {
            int sum = a + b;

            return sum;
        }

        public static int Raz(int a, int b)
        {
            int raz = a - b;

            return raz;
        }

        public static int Pro(int a, int b)
        {
            int pro = a * b;

            return pro;
        }

        public static int Chas(int a, int b)
        {
            int chas = a / b;

            return chas;
        }
    }
}

# Скриншот

![image](https://user-images.githubusercontent.com/59621706/228197685-39d21653-1a3e-4889-a0fa-73ae073c99b6.png)

![image](https://user-images.githubusercontent.com/97594467/230591988-aea7fe0d-d5be-48ac-8565-148679a3577c.png)

