---
# Оставьте заголовок главной страницы пустым, чтобы использовать заголовок сайта
title: "heroincult4r4r"
date: 2022-10-24
type: landing

design:
  # Стандартный отступ между секциями
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Выберите профиль пользователя для отображения (имя папки в `content/authors/`)
      username: admin
      text: ""
      # Показать кнопку призыва к действию под биографией? (опционально)
      button:
        text: Скачать резюме
        url: uploads/resume.pdf
    design:
      css_class: dark
      # Настройка аватара
      avatar:
        size: medium  # Варианты: small (150px), medium (200px, по умолчанию), large (320px), xl (400px), xxl (500px)
        shape: circle # Варианты: circle (по умолчанию), square, rounded
      background:
        color: black
        image:
          # Добавьте фоновое изображение в `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Мои исследования'
      subtitle: ''
      text: |-
        Моя научная деятельность сосредоточена на междисциплинарных исследованиях 
        на стыке поп-культуры и глобальной политики. В настоящее время я провожу 
        глубокое научное исследование о связи феномена Лабубу с геополитическими 
        процессами и структурами Пентагона.

        Используя методы критического дискурс-анализа и семиотики, я исследую, 
        как виниловые игрушки становятся инструментами мягкой силы и культурного 
        влияния в международных отношениях. Особое внимание уделяется анализу 
        скрытых нарративов и символических кодов в дизайне коллекционных фигурок.

        Готов к междисциплинарному сотрудничеству с политологами, культурологами 
        и специалистами по международным отношениям!
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Избранные публикации
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Последние публикации
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Последние и предстоящие выступления
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Последние новости
      subtitle: ''
      text: ''
      # Тип страницы для отображения. Например: post, talk, publication...
      page_type: post
      # Выберите, сколько страниц отображать (0 = все страницы)
      count: 5
      # Фильтр по критериям
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Выберите смещение для страниц
      offset: 0
      # Порядок страниц: по убыванию (desc) или возрастанию (asc) даты.
      order: desc
    design:
      # Выберите вид layout
      view: date-title-summary
      # Уменьшить отступы
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Отображать эту секцию только на демо-сайте Hugo Blox Builder
    content:
      title: 👉 Создайте свой собственный академический сайт как этот
      text: |-
        Этот сайт создан с помощью Hugo Blox Builder - БЕСПЛАТНОГО конструктора сайтов на основе Hugo, которому доверяют более 250 000 академиков, как и вы.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Легко создавайте что угодно с помощью блоков - без необходимости написания кода!
        
        От целевых страниц, вторых мозгов и курсов до академических резюме, конференций и технических блогов.
      button:
        text: Начать
        url: https://hugoblox.com/templates/
    design:
      card:
        # Цвет фона карточки (CSS класс)
        css_class: "bg-primary-700"
        css_style: ""
