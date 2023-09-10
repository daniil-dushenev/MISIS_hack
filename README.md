<h1 align="center">MISISInder</h1>

<img class="left-align-img" src="https://github.com/daniil-dushenev/MISIS_hack/blob/main/logo.png" alt="Ваше изображение">

### Сервис, который поможет ребятам найти друзей в НИТУ МИСИС
Проект создан с целью помочем людям найти новые знакомства в стенах университета.
При запуске тг-бота нужно пройти анкетирование и написать немного о себе для того чтобы рекоменадтельная система максимально точно подобрала человека с похожими интересами


### Режимы
1) Поиск похожего человека с помощью рекоммендательной системы(описана ниже)
2) Поиск противоположного человека с помощью рекоммендательной системы(Сделанно в случае если вы захотите расширить кругозор)
3) Совершенно случайный пользователь
4) Поиск по категориям(Например: вы хотите изучить интегралы и тогда вы выбираете категорию "математика", система подбирает человека, который тоже хочет изучать математику. Аналогично со студ. объединениями, институтом)

### Как это работает?
Рекомендательная система использует информацию про специализации, которые пользователь выбрал и текстовое описание целей, хобби юзера.
В качестве рекомендательной системы мы используем усреднение косинусного растояния между векторами текста анкеты и косинусного растояния между векторами интересов(хобби)
Для создания векторов описания мы используем Sentence Bert, а для для создания векторов интересов One Hot Encoding
