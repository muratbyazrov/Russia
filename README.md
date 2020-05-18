# Russia - сайт о путешествии по России
### [Посмотреть можно тут](https://muratbyazrov.github.io/Russia/)

## Что интересного?
Этот сайт полностью резиновый. Благодаря медиазапросам сайт корректно работает на всех типах устройств, начиная от широких мониторов и заканчивая экарном смартфона

## Какие технологии? 
- HTML
- CSS

## А что конкретно? 
### Семантика
Соблюдена семантика
Для вёрстки заголовков применяются несколько тегов от h1 до h6, текстовые блоки размечены тегами p, списки — ul. Присутствуют и используются по назначению элементы header, main, footer, section, nav.
Заголовки, параграфы и текстовый контент дополнительно не обёрнуты в div, например:
<div><p>Text here</p></div>.
Для переноса текста и создания отступов не используется элемент br. ####

### БЭМ
Файловая структура по БЭМ.
Нет классов, содержащих в названии только БЭМ-модификатор. Например,
<div class='block__element_mod-name_mod-value>.
Правильно — <div class='block__element block__element_mod-name_mod-value>.
Отсутствуют классы с числовыми значениями, либо отражающие позицию элемента.
Например, <div class='block__first block__1>
Компоненты со стилевым и логически похожим оформлением выделены в одну БЭМ-сущность: блок или элемент.
Используется БЭМ-модификатор для подчёркивания одного из языков.
  
### Доступность интерфейса
Все ссылки и интерактивные элементы имеют состояние наведения :hover.
Контентные изображения имеют alt с корректным описанием, соответствующим языку страницы.  

### CSS
Контент на странице отцентрован.
Для установки размеров и отступов выбраны относительные величины и подходящие CSS-свойства. Например, max-width лучше использовать для текстовых элементов, нежели width.
Ни одному текстовому блоку не задана фиксированная высота. Блок растягивается, если в него вставляют в 2—3 раза больше текста.
Установлен серый фон для всей страницы, нет белых полей по бокам.
Подключены системные шрифты для случаев, когда основной не загрузился.
У элементов с абсолютным позиционированием заданы координаты по двум осям.
Затемняется изображение при :hover на любую область блоков video или cover (в т. ч. и при наведении на текстовые элементы).
Отсутствует горизонтальная прокрутка при изменении ширины окна просмотра в отладчике.
Брейкпоинты сгруппированы.
Проект визуально соответствует макетам. Корректно отображается вёрстка на разрешениях, предусмотренных макетами.
Одинаковые свойства в разных медиа-правилах не дублируются. В каждом медиа-правиле описаны только те стили, которые отличаются от другого медиа-правила.
