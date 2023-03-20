# How to learn
==============
# Учебный проект по верстке
***Содержание:***
- [Введение](#Introduction)
- [Описание проекта](#Project-description)
- [Планы по доработке](#Plans-to-refine)

# Введение <a name="Introduction"></a>

**How to learn** - проект, созданный по ходу изучения темы "Верстка сайтов" на Яндекс.Практикум. Основная цель - дать советы по обучению, чтобы улучшить усваиваемость материала. В проекте представлены различные техники обучения от известных людей, обучающие видеоролики и множество интересных фактов об учебе.

Более подробное описание функционала представлено ниже:

# Описание проекта <a name="Project-description"></a>
В проекте рассмотрены основные проблемы обучения и способы их решения. Конкретные техники и упражнения помогают изменить подход к обучению, сделать его эффективным и захватывающим, что в последствии можно будет применить во всех сферах жизни. Все советы представлены в интересном для читателя формате и сопровождаются соответствующими фотографиями и примерами. 
Благодаря фото, видео и анимациям, которые представлены в проекте, пользователь не будет уставать от однотонного текста, а значит и материал будет усваиваться намного приятнее и быстрее. Почти каждое из упражнений сопровождается ссылками на полезные материалы, которые помогут глубже понять тему.

**How to learn** представляет из себя одностраничный сайт, написанный на *HTML*, где за стили элементов и анимации отвечает *CSS*. 
Все анимации реализованы с помощью *@keyframe* и подключаются миксом:
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
Видео в проекте реализованы с помощью *iframe*:
```
<iframe class="video__iframe" src="https://www.youtube.com/embed/arj7oStGLkU" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe class="video__iframe" src="https://www.youtube.com/embed/5MgBikgcWnY" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```
