# How to learn
==============
# Учебный проект по верстке
***Содержание:***
- [Введение](#Introduction)
- [Описание проекта](#Project-description)
- [Планы по доработке](#Plans-to-refine)

# Введение <a name="#Introduction"></a>

**How to learn** - проект, созданный по ходу изучения темы "Верстка сайтов" на Яндекс.Практикум. Основная цель - дать советы по обучению, чтобы улучшить усваиваемость материала. В проекте представлены различные техники обучения от известных людей, обучающие видеоролики и множество интересных фактов об учебе.

Более подробное описание функционала представлено ниже:

# Описание проекта <a name="Project-description"></a>
В проекте рассмотрены основные проблемы обучения и способы их решения. Конкретные техники и упражнения помогают изменить подход к обучению, сделать его эффективным и захватывающим, что в последствии можно будет применить во всех сферах жизни. Все советы представлены в интересном для читателя формате и сопровождаются соответствующими фотографиями и примерами. 
Благодаря фото, видео и анимациям, которые представлены в проекте, пользователь не будет уставать от однотонного текста, а значит и материал будет усваиваться намного приятнее и быстрее. Почти каждое из упражнений сопровождается ссылками на полезные материалы, которые помогут глубже понять тему.

**How to learn** представляет из себя одностраничный сайт, написанный на *HTML*, где за стили элементов и анимации отвечает *CSS*. 

Все файлы в проекте организованы согласно *БЭМ Nested*. Все блоки и элементы разбиты по соответствующим папкам, что позволяет изпользовать многие блоки повторно в других секциях. Например, блок *table* используется дважды, в различных секциях.

Сама страница разбита на множество секций, что позволяет постоянно дорабатывать и улучшать сайт, добавлять новые элементы и даже разделы.

Анимации реализованы с помощью *@keyframe* в отдельном блоке и подключаются миксом:
```
@keyframes rotate{
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}
```

```
<div class="header__square-pic rotation"></div>
```
Такой подход позволяет ипользовать анимации для различных элементов, что заметно уменьшает количество кода:

```
<div class="kaufman__triangle rotation"></div>
```

Видео в проекте реализованы с помощью *iframe*:
```
<iframe class="video__iframe" src="https://www.youtube.com/embed/arj7oStGLkU" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe class="video__iframe" src="https://www.youtube.com/embed/5MgBikgcWnY" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```

Ссылки в проекте кликабельны и переносят пользователя в новое окно, не закрывая текущее. Такой подход упрощает работу с сайтом для его пользователей.
Также при наведении на них, меняется их *opacity*:
```
.feynman__link:hover{
  opacity: 0.33;
  transition: all 0.2s ease-out;
}
```

Почти все таблицы реализованы с помощью списков:
```
<ul class="footer__column-links">
  <li class="footer__list-item"><a href="#" class="footer__column-link">Главная</a></li>
  <li class="footer__list-item"><a href="#" class="footer__column-link">Концепция</a></li>
  <li class="footer__list-item"><a href="#" class="footer__column-link">Наставники</a></li>
</ul>
```
Такой подход позволяет сделать код читабельнее и проще в доработке.

В разделе *footer* иконки являются частью ссылки, что позволяет пользователю нажимать и на них
```
<a href="https://www.youtube.com/" target="_blank" class="footer__column-link">
  <img src="images/youtube-icon.svg" alt="ютуб" class="footer__social-icon">Youtube
</a>
```

# Описание проекта <a name="Plans-to-refine"></a>
