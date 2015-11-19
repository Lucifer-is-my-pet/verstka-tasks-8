# Задача к лекции «Анимации» – «айБабулька»

:sos: [Как создать Pull Request](https://github.com/urfu-2015/guides/blob/master/how-to-pull-request.md)  
:warning: [Codestyle для HTML](https://github.com/urfu-2015/guides/blob/master/html-codestyle.md)  
:warning: [Codestyle для CSS](https://github.com/urfu-2015/guides/blob/master/css-codestyle.md)  
:warning: При создании PullRequest'а не забудьте указать ваши имя и фамилию.

### Общие требования

Мы очень хотим, чтобы код вы написали сами на чистом CSS и HTML, а __не пользовались внешними библиотеками, пост и препроцессорами__.

Прежде чем отправлять решение, проверьте его на соответствие [требованиям к HTML коду](https://github.com/urfu-2015/guides/blob/master/html-codestyle.md)   
и [требованиям к CSS](https://github.com/urfu-2015/guides/blob/master/css-codestyle.md).

Когда вы создадите или обновите пулл-реквест, он частично будет проверен
автоматически. Результаты вы увидите внизу:

Если всё хорошо:  
<img width="308" alt="2015-10-08_1845" src="https://cloud.githubusercontent.com/assets/4534405/10368030/ccc43228-6dec-11e5-925e-47793862d13e.png">

Если всё плохо:  
<img width="218" alt="2015-10-08_1841" src="https://cloud.githubusercontent.com/assets/4534405/10367916/60487fc8-6dec-11e5-9e1d-2a1b15da2220.png">

Проверить HTML и CSS можно и вручную:
```sh
# Устанавливаем проверяльщик
npm install

# Проверяем
npm test

# В результате выведутся ошибки, если они есть.
# Если какие-либо ошибки будут не понятны – смело спрашиваем у ментора.
```

В помощь вам мы разместили файл `.editorconfig`. Этот файл содержит базовые
правила оформления кода (codestyle), понятные для большинства редакторов.
Прочитайте [о нём подробнее](https://github.com/urfu-2015/guides/blob/master/editorconfig.md).

### Задача

Витрина лучших экземпляров осеннего урожая пользуется популярностью и одна грушевая компания обратила на нее внимание. Эта компания готова рекламировать продукцию бабуленек за скромные три ящика моркови.

Однако, для запуска рекламной кампании необходимо сверстать 3D галерею продуктов. Это обязательное условие грушевой компании и никакие овощные «подарки» не изменят их решение. Придется постараться.

<a href="https://cloud.githubusercontent.com/assets/4165695/11270678/bc99db5c-8ee2-11e5-95ea-368584ff3f83.png" target="_blank">
    <img width="300" src="https://cloud.githubusercontent.com/assets/4165695/11270678/bc99db5c-8ee2-11e5-95ea-368584ff3f83.png">
</a>

**Обязательное задание**

* На странице отображается 7 фотографий (макет №1)
* Фотография по центру (активная) отображается без искажения на переднем фоне
* Фотографии слева и справа от активной «повернуты» к ней и находятся «позади» нее
* Необходимо добиться ощущения 3D пространства
    * Активная фотография находиться в плоскости экрана
    * Неактивные фотографии «отодвинуты» от плоскости экрана «вглубь» на одинаковое расстояние 
    * Чем дальше фотография от активной - тем меньше ее поворот
* При клике на неактивную фотографию - она становится активной (макет №2)
    * Происходит анимированное перемещение фотографии в центр
    * При перемещении фотография постепеннно теряет искажение и в конечном итоге располагается в плоскости экрана в «стандартном» 2D виде
    * Остальные фотографии перемещаются вслед за новой активной
    
__Задание необходимо решить без использования JS и с использованием CSS преобразований и переходов/анимаций__

### Необязательное задание (+15 к массе)

Бабуленька хорошо следит за своим огородом и он благодарит ее большим урожаем. Не все удается продать и часть продуктов остается в доме. Бабуленька любит угощать внучка всяческими овощными изысками.

Из каждого овоща хозяйка может приготовить вкуснейшее фирменное блюдо, например, кабачковые оладушки. Только наш внучок имеет счастье отведать такие оладушки и это нужно исправить.

При наведении на активную фотографию (и только на нее) у нас появляется ссылка на рецепт блюда из этого овоща (макет №3).

Анимацию появления ссылки на рецепт вы можете придумать сами.

При клике на эту ссылку карточка плавно разврачивается к нам «задней» стороной и увеличивается (создавая эффект «полета» к нам на встречу из экрана, макеты №4-6). Мы видим название блюда и рецепт (макет №7).

По клику на крестик анимация воспроизводится в обратном направлении, возвращая слайдер к состоянию до клика.

__Дополнительное задание необходимо решить без использования JS и с использованием CSS преобразований и переходов/анимаций__

![Откормленные внуки](https://cloud.githubusercontent.com/assets/4165695/11269790/442a5dba-8edb-11e5-9c1a-194fe2e9bed9.jpeg)

:warning: При разработке 3D галереи ни один внук не остался голодным
