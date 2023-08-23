# vue-toggle-dark-theme
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/shtekleinmax/vue-toggle-dark-theme/blob/main/README.md)
[![ru](https://img.shields.io/badge/lang-ru-red.svg)](https://github.com/shtekleinmax/vue-toggle-dark-theme/blob/main/README.ru.md)

Простой переключатель тёмной/светлой темы

# Демонстрация
https://maxweb.kz/toggle-dark-theme/

# Особенности
- только 2 режима: тёмный и светлый
- выбранный режим сохраняется в LocalStorage (переменная "dark-mode") и используется при следующей загрузке сайта
- когда сайт загружается в первый раз настройки темы берутся из настроек браузера
- используется метатег `<meta name="theme-color" content="">` для стилизации браузера (подробнее: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name/theme-color)

# Использование
1. Добавьте этот компонент в ваш проект
2. Вызовите при помощи `<toggle-dark-theme />`

# Настройки
| Опция        | Тип          | Значение по умолчанию       | Описание   |
| ------------- | ------------- | ------------- | ------------- |
| buttons       | Object        | {dark: "Dark mode", light: "Light mode"} | Текст переключателя. Для каждого режима отдельно |
| colors        | Object        | {dark: "#0b2137", light": "#ffffff"} | Цвет для каждого режима. Используется в `<meta name="theme-color" content="">` |

# Пример
```JS
<toggle-dark-theme
      :buttons = '{
          dark: "Enable dark theme",
          light: "Enable light theme"
      }'
      :colors = '{
          dark: "#0b2137",
          light: "#ffffff"
      }'
  />
```
