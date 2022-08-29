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

<!-- heder menu __portfolio -->

<header class="header">
      <div class="container container-nav">
        <nav class="navigasion">
          <a class="logo" href="./index.html">
            <span class="span__logo">Web</span
            ><span class="span__studio span__studio--color-dark"
              >Studio</span
            ></a
          >
          <ul class="navigasion__list header__list list">
            <li class="navigasion__item">
              <a href="./index.html" class="navigasion__link">Студия</a>
            </li>
            <li class="navigasion__item">
              <a href="" class="navigasion__link active">Портфолио</a>
            </li>
            <li class="navigasion__item">
              <a href="" class="navigasion__link">Контакты</a>
            </li>
          </ul>
        </nav>
        <ul class="contacts contacts__list list">
          <li class="contacts__item">
            <a href="mailto:info@devstudio.com" class="contacts__conect"
              ><svg class="contacts__icon" width="10" height="16">
                <use href="./imag/symbol-defs.svg#icon-envelope"></use></svg
              >info@devstudio.com</a
            >
          </li>
          <li class="contacts__item">
            <a href="tel:+380961111111" class="contacts__conect"
              ><svg class="contacts__icon" width="10" height="16">
                <use href="./imag/symbol-defs.svg#icon-smartphone"></use></svg
              >+38 096 111 11 11</a
            >
          </li>
        </ul>
      </div>
    </header>

<!-- Heder scss -->

.header {
position: relative;
background-color: #ffffff;
border: 1px solid #eeeeee;
}

.container-nav {
}
.navigasion {
display: flex;
align-items: center;
justify-content: space-between;
width: 100%;
}
.menu-btn {
background-color: #fff;
color: #000;
cursor: pointer;
border: none;
padding: 0;
margin: 0;
display: inline-flex;

transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
color 250ms cubic-bezier(0.4, 0, 0.2, 1);
&:hover {
fill: #2196f3;
}
& .icon-cross {
display: none;
}
&.is-open .icon-cross {
display: block;
}
&.is-open .icon-menu {
display: none;
}
@media screen and (min-width: 768px) {
display: none;
}
}

.menu-container {
background-color: #fff;
@media screen and (max-width: 767px) {
display: none;
position: absolute;
top: 100%;
left: 0;
width: 100%;
padding: 40px;
&.is-open {
display: block;
}
}
@media screen and (min-width: 768px) {
display: flex;
justify-content: space-between;
flex-grow: 1;
}
}

.navigasion**list {
@media screen and (max-width: 767px) {
margin-bottom: 300px;
}
@media screen and (min-width: 768px) {
display: flex;
margin-left: 95px;
& .navigasion**item + .navigasion**item {
margin-left: 50px;
}
}
}
.navigasion**link {
position: relative;
display: block;
padding-top: 16px;
padding-bottom: 16px;

text-decoration: none;
color: #212121;
font-weight: 500;
font-size: 40px;
line-height: 1.14;
letter-spacing: 0.02em;
cursor: pointer;
transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
&:hover,
&:focus {
color: #2196f3;
}
@media screen and (min-width: 768px) {
padding-top: 35px;
padding-bottom: 35px;
font-size: 14px;
}
}

// --------------- contacts ---------------

/_ header ссылки емеил и тел _/

.contacts\_\_list {
@media screen and (min-width: 768px) {
display: flex;
flex-direction: column-reverse;
// margin-left: 85px;

    // justify-content: end;

}
@media screen and (min-width: 1200px) {
display: flex;
flex-direction: row;
align-items: center;
gap: 30px;
}
}

.contacts\_\_conect {
display: flex;
align-items: center;
font-style: normal;
font-weight: 500;
font-size: 14px;
line-height: 1.14;
letter-spacing: 0.02em;
color: #757575;
// padding-top: 35px;
// padding-bottom: 35px;
padding-top: 16px;
padding-bottom: 16px;
transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
&:hover,
&:focus {
color: #2196f3;
transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
@media screen and (min-width: 768px) {
padding-top: 10px;
padding-bottom: 10px;
}
}

.contacts**tel {
@media screen and (max-width: 767px) {
font-size: 34px;
color: #2196f3;
}
}
.contacts**mail {
@media screen and (max-width: 767px) {
font-size: 24px;
margin-bottom: 65px;
}
}
.contacts**icon {
margin-right: 10px;
fill: #757575;
height: 16px;
width: 20px;
fill: currentColor;
&:hover,
&:focus {
color: #2196f3;
transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
@media screen and (max-width: 767px) {
display: none;
}
}
.heder-cocials {
@media screen and (max-width: 767px) {
display: flex;
gap: 20px;
width: 100%;
flex-wrap: wrap;
}
@media screen and (min-width: 768px) {
display: none;
}
}
.heder-cocials**link {
color: #2196f3;
font-style: normal;
font-weight: 500;
font-size: 18px;
line-height: 1.2;
letter-spacing: 0.02em;
}
