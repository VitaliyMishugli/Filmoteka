First!!!!

Щоб запустили термінал використовуємо комбінацію ctrl+j на Windows.

1. Встановити всі залежності (ініціалізувати проект) в терминалі команда
   `npm install`. Перевірити чи з'явилась папка node_modules
2. Що запустити розробку виконай в терміналі команду `npm start`.
3. Перейди в браузере по адресу [http://localhost:1234] і go.

Info!!!!

JS

В кожній папці наприклад js є підпапки які будуть називатись - ім'я
папки-index.js. Підключаємо нові файли js тільки в ці файли. В свою чергу
налаштовано в папці js є main.js в які підключені файли ім'я папки-index.js в
які підключені всі файли з підпапок. І файл main.js з папки js підключений до
index.js в src.

ВСЕ ЩО НЕ ВІДНОСИТЬ ДО API, COMMON, DOM додаємо в Other імпорти підключаємо в
other-index.js.

HTML

src/partials створюємо необхідні html файли та додаємо імпорти до файлу
partials-index.html. Який підключений до основного index.hml в src.

SASS

В кожній підпапці є свій ім'я-index.scss в які підключаємо всі імпорти з данної
папки. ім'я-index.scss додані до index.scss.

Додано: Body styles. Container. Resets. Components : Можемо створювати файли зі
стилями на кнопку, модалку, та інше. Layouts: Папка для стилізації html. Utils:
Створено mixin для line-height та font-size, як використовувати : @include
lh(16px, 12px, 12px); Vars: прошу звернути особливу увагу, використовуємо
функції getColor(тут колір з colors); getSize(desktop(тут назву з breakpoints))
Приклади використання:

@media screen and (min-width: getSize(tablet)) / background-color:
getColor(white-text-color); / color: getColor(primary-text-color); / transition:
color getProperty(time) getProperty(cubic);

............................................................................................

! Section header "Rostyslav Kviatkovskyi"

1. FT-01 Зверстати хедер головної сторінки (мобілка, планшет, робочий стіл) {
   html: src/partials/header / images: src/images/header }
2. FT-12 Зверстати хедер для сторінки "My Library" (мобілка, планшет, робочий
   стіл)
3. FT-13 Після натискання на логотип відображається головна сторінка
4. FT-02 За натисканням на логотип/кнопку "Home" відображається головна сторінка
5. FT-03 За натисканням на кнопку "My Library" відображається бібліотека
   користувача
6. FT-10 Реалізувати пошук та відображення фільмів за ключовим словом

! Section foother "Tetiana Bulatova"

1. FT-04 Верстка футера (мобілка, планшет, десктоп) (однаковий для двох
   сторінок)
2. FT-23 Зверстати модалку (мобілка, планшет, десктоп) з інформацією про
   учасників вашої команди, яка відкриватиметься натисканням на текст "GoIT
   Students" у футері

!"Yaroslav Taranovskiy"

API/AXIOS/Запити Написати всі axios.get src/js/ api

1. запит повної інформації про кінофільм для сторінки кінофільму,
2. запит на список найпопулярніших фільмів на сьогодні для створення колекції на
   головній сторінці:

! "Віталій Мішуглі" src/js/dom - create-movie-markup.js

1. FT-07 Реалізувати підвантаження популярних фільмів на головну (першу)
   сторінку
2. FT-05 Зверстати шаблон картки одного фільму

! "Юра Погорілець" src/js/common - pagination.js/ src/partials pagination.html/
scss


1. FT-08 Зверстати чи підключити номери сторінок (пагінація) на головній
   сторінці
2. FT-09 При переході на кожну сторінку малювати відповідну частину фільмів
3. FT-21 Підключити/зверстати Loader (spinner) для асинхронних запитів

! "Diana Pustolyakova" src/partials /library-collection/ header-library

1. FT-11 Зверстати контейнер сторінки "My Library" для правильного
   позиціонування карток фільмів (мобілка, планшет, робочий стіл)
2. FT-06 Зверстати контейнер головної сторінки для правильного позиціонування
   карток фільмів (мобілка, планшет, робочий стіл)

! "Віталій Поляков" src/js/dom - queue.js / watched.js

1. FT-14 За натисканням на кнопку "Watched" показуються переглянуті фільми
   користувача
2. FT-15 За натисканням на кнопку "Queue" показуються фільми додані в чергу
   користувача

! "Александр Чигрин" src/js/dom - movie-modal.js доданий код модалки з ft-20

1. FT-16 Зверстати шаблон модалки одного фільму (мобілка, планшет, робочий стіл)
2. FT-20 Реалізувати закриття модалки за натисканням на клавішу ESC і за кліком
   поза межами модалки, не забути зняти слухачів
3. FT-17 Після натискання на картку фільму на будь-якій сторінці повинна
   відкриватися модалка з динамічно підставленою інформацією про фільм

! "Олексій Колесник"

1. FT-18 За натисканням на кнопку "Add to watched" фільм додається до
   переглянутих фільмів поточного користувача (local-storage)
2. FT-19 За натисканням на кнопку "Add to queue" фільм додається до черги
   поточного користувача (local-storage)

! "Андрій Степанюк" src/js/other - localeStrageServices src/partions -
spinner.html/scss

1. Реалізувати запит по трейлерам та підключити трейлер до модального вікна
2. FT-22 To top, скрол на верх
# Filmoteka