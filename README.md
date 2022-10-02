Если вы хотите использовать изображение в качестве фона CSS, есть изящное решение. Просто используйте cover или contain в свойстве background-size CSS3.

<div class="container"></div>​

.container {
    width: 150px;
    height: 100px;
    background-image: url("http://i.stack.imgur.com/2OrtT.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: 50% 50%;
}​
Пока cover даст вам увеличенное изображение, contain даст вам уменьшенное изображение. Оба сохраняют соотношение сторон пикселей.

<http://jsfiddle.net/uTHqs/> (с использованием обложки)

<http://jsfiddle.net/HZ2FT/> (с использованием файла)

Этот подход имеет то преимущество, что он дружелюбен к дисплеям Retina в соответствии с быстрым руководством Томаса Фукса. <http://cl.ly/0v2u190o110R>

Стоит отметить, что поддержка браузера для обоих атрибутов исключает IE6-8. <http://www.quirksmode.org/css/background.html>
