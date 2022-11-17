<h1>Классификация изображений на основе сверточных нейронных сетей</h1>
<h2>Входящие файлы</h2>
<li>4140_CV_ЛР3_Строкова_AlexNet.ipynb - ноутбук с программным кодом на Python;
<li>4140_CV_ЛР3_Строкова_GoogleNet.ipynb - ноутбук с программным кодом на Python;
<li>4140_CV_ЛР3_Строкова_VGG16.ipynb - ноутбук с программным кодом на Python;
<li>4140_CV_ЛР2_Строкова.pdf - текстовый отчет;
<li>Каталог "Изображения" - исходные изображения.
<h2>Постановка задачи</h2>
Цель работы: научиться создавать простые системы классификации изображений на основе сверточных нейронных сетей. <br>
<br>
Базовый алгоритм: классификация.<br>
<br>
Задание: на вход поступает два изображения: на вход поступает изображение, которое преобразуется в нужный для обработки моделью нейронной сети формат (тензор), выполняется предобработка (при необходимости – изменение размера и нормирование), затем обрабатывается с помощью нейронной сети и выводится результат (номер класса, название, вероятность для первых 5-ти наиболее вероятных классов). <br>
<br>
Задачи: 
<li> реализовать систему классификации через AlexNet;
<li> реализовать систему классификации через GoogleNet;
<li> реализовать систему классификации через VGG16;
<li> сравнить качество работы, скорость и количество потребляемой памяти для каждой архитектуры.
<br>
<h2>Теоретическая база</h2>
Для решения задачи классификации изображений используются сверточные нейронные сети. Набор изображений следующий:<br>
<br>
   Медведи:<br>
<img src="Изображения/1.jpg"/ width="100" height="80">

<h2>AlexNet</h2>
Нейронная сеть AlexNet:
<li> архитектура данной сети похожа на LeNet, но она глубже (8 слоев – 5 сверточных и 3 полносвязных);
<li> впервые была использована ReLU в качестве функции активации (вместо арктангента);
<li> при обучении был использован dropout (вместо регуляризации).
<br>
Сеть включает в себя свертки, максимальное объединение, dropout, аугментацию данных, функции активаций ReLu и стохастический градиентный спуск. Обучение происходило на ImageNet (15 миллионов помеченных изображений с высоким разрешением, разделенных на 22 000 категорий).<br>
<br>
Первые пять слоев сверточные, остальные три – полносвязные. ReLu применяется после каждого сверточного и полносвязного слоя. Dropout применяется перед первым и вторым полносвязным слоями. Обучение проходит 90 эпох, скорость обучения 0,01.<br>
<br>
<img src="Изображения/Прямой_поиск/0.png"/>

<h2>GoogleNet</h2>
Нейронная сеть GoogleNet:
<li> архитектура данной сети...;
<li> функция активации...;
<br>
Сеть включает в себя .... Обучение происходило на ....<br>
<br>
Текст, текст, текст. <br>
<br>
<img src="Изображения/Прямой_поиск/0.png"/>
Текст, текст, текст. <br>

<h2>VGG16</h2>
Нейронная сеть VGG16:
<li> архитектура данной сети...;
<li> функция активации...;
<br>
Сеть включает в себя .... Обучение происходило на ....<br>
<br>
Текст, текст, текст. <br>
<br>
<img src="Изображения/Прямой_поиск/0.png"/>
Текст, текст, текст. <br>

<h2>Выводы по работе</h2>
Проведена классификация пользовательского датасета изображений с использованием предобученных сверточных нейронных сетей: AlexNet, GoogleNet, VGG16.<br>
<br>
На вход подавались 50 фотографий (скачаны с сети Интернет и сделаны самостоятельно). На выходе алгоритм выдавал изображение, которое классифицировалось, и 5 вероятностей отнесения фотографии к определенному классу. Можно заметить, что ... дает лучшие результаты. <br>
<br>
Составим сравнительную таблицу, чтобы продемонстрировать верные и неверные ответы нейронной сети. Для подсчета итоговых баллов будем использовать трех бальную шкалу, где 2 – верно (верный ответ находится в ТОП-1), 1 – неверно частично (верный ответ находится в ТОП-5, но не в ТОП-1), 0 – неверно (алгоритм предлагает неверные ответы классификации).<br>
<br>
<table border="1">
   <tr>
    <th>№</th>
    <th>Описание изображения</th>
    <th>Ожидаемый класс</th>
    <th>AlexNet</th>
    <th>GoogleNet</th>
    <th>VGG16</th>
   </tr>
 </table>
Таким образом, мы видим, что ...
