# HM-1-desktop

transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
color 250ms cubic-bezier(0.4, 0, 0.2, 1);

transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);

/_ .portfolio-tumb::before {
display: inline-block;
position: absolute;
content: '';
width: 100%;
height: 100%;
background-color: rgba(33, 150, 243, 0.9);
transform: translateY(100%);
opacity: 0;
} _/

/_ селекторы _
/_ универсальный _
тега - p
кнопки и teg adress не унаследуют шрифт надо вручную
id используетс ядля ссылки в тесте при нажатии перекинут на то место где это необходимо ЕГО не используем - # text

клас (. css) (class - html) самі популярній но проблема вибирать название класса
h1,h2,h3 - title
p - text
nav - navigatia
list- список ul
item - єлемент списка li
link - ссылка
атрибут
[href] все ссілки відялятся в той цвет которій зададим
[href] {
color: aqua; }
дочерний .team > p {
color: rgb(172, 239, 16); }
потомка
.team p {
color: rgb(172, 239, 16); }
\*/
/_ задал цвет рамки.header-item {
outline: 1px solid red;
} _/

/_ крайняя геометрия.
Всем едлементом с класом item которіе находятся внутри header-list
не являются последними детьми в своей коллекции_/

/_ .header-list .header-item:not(:last-child) {
margin-right: 50px;
} _/
.portfolio-list {
display: flex;
flex-wrap: wrap;
/_ justify-content: space-between; _/
gap: 10px;
padding: 0;
list-style: none;
background-color: yellowgreen;
}

.portfolio-item {
/_ width: calc((100% - 60px) / 3); _/
margin-right: 30px;
margin-bottom: 30px;
}
.portfolio-item:nth-child(3n) {
margin-right: 0;
}

.portfolio-item:nth-last-child(-n + 3) {
margin-bottom: 95px;
}

<!-- ---изменение цвета с помощью currentColor--- -->

.item-soc-link {
width: 44px;
height: 44px;
border-radius: 50%;
background-color: rgb(181, 232, 233);
/_ background-color: #ffffff; _/
display: flex;
align-items: center;
justify-content: center;
color: #afb1b8; - цвет задали для унаследования
}
**\_\_**унаследование при каждом изменении ывета\_\_\_\_
.item-soc-icon {
fill: currentColor;
}

.item-soc-link:hover,
.item-soc-link:focus {
background-color: #2196f3;
color: #ffffff;
}
/\* .item-soc-icon {
fill: currentColor;
}

.item-soc-link:hover,
.item-soc-link:focus {
background-color: #2196f3;
color: #ffffff;
} _/
/_ .item-soc-icon {
fill: #afb1b8;
} _/
/_ .item-soc-link:hover,
.item-soc-link:focus {
background-color: #2196f3;
} _/
/_ .item-soc-link:hover .item-soc-icon {
fill: #ffffff;
} \*/

<a href="" class="header-icon">
              <svg class="header-tel-icon" width="20" height="20">
              <use href="./imag/symbol-defs.svg#icon-smartphone"></use>
              </svg>
              </a>
<a href="" class="header-icon">
              <svg class="header-tel-icon" width="20" height="20">
              <use href="./imag/symbol-defs.svg#icon-envelope"></use>
              </svg>
              </a>
./imag/symbol-defs.svg#icon-envelope

.benefits-item::before {
display: block;
content: '';
height: 120px;
margin-bottom: 30px;
background-repeat: no-repeat;
background-position: center;
background-color: #f5f4fa;
border-radius: 4px;
}
.icon-antena::before {
background-image: url(../imag/antenna.svg);
}
.icon-clok::before {
background-image: url(../imag/clock.svg);
}
.icon-diagram::before {
background-image: url(../imag/diagram.svg);
}
.icon-astronaut::before {
background-image: url(../imag/astronaut.svg);
}
