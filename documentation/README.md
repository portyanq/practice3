# Документация по шорткодам

### First Shortcode
В первом шорткоде, необходимо напрямую передавать переменные. Пример вызова шорткода:

```
---
title: "First"
date: 2022-02-24T23:36:53+03:00
draft: false
---

{{< first_snippet 

    teacher_about = "Преподаватель Английского Языка" 

    teacher_photo_url = "https://htmlstream.com/unify/assets/img/160x160/img10.jpg"

    teacher_description = "Хорошая учительница с огромным стажем образования"
    
>}}
```


### Second Shortcode
Для второго шорткода было принято решение использовать .json файл, где будет хранится информация о генерируемых карточках.
```

{
    "title": "Наши лидеры",
    "cardsData": [
        {
            "img_link": "https://htmlstream.com/unify/assets/svg/brands/google-dark.svg"
        },
        {
            "img_link": "https://htmlstream.com/unify/assets/svg/brands/amazon-dark.svg"
        },
        {
            "img_link": "https://htmlstream.com/unify/assets/svg/brands/forbes-dark.svg"
        },
        {
            "img_link": "https://htmlstream.com/unify/assets/svg/brands/business-insider-dark.svg"
        },
        {
            "img_link": "https://htmlstream.com/unify/assets/svg/brands/shopify-dark.svg"
        }
    ]
}
```

### Third Shortcode
В третьем шорткоде, как и в первом, используется файл с данными:
```
---
title: "Third"
date: 2022-02-26T23:40:04+03:00
draft: false
---

{{< third_snippet 
    main_text = "Мы будем рады с вами сотрудничать"
    more_info_descr = "Свяжитесь с нами"
>}}
```