# vue-toggle-dark-theme
[![ru](https://img.shields.io/badge/lang-ru-red.svg)](https://github.com/shtekleinmax/vue-toggle-dark-theme/blob/main/README.ru.md)

A simple light/dark site theme switcher.

# Demo
https://maxweb.kz/toggle-dark-theme/

# Features
- 2 modes only: light and dark
- the selected mode is stored in LocalStorage ("dark-mode" variable) and used the next time the site is loaded.
- when the site is loaded for the first time, the mode settings are taken from the browser settings
- uses the `<meta name="theme-color" content="">` to style the browser (more info: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name/theme-color)

# Using
1. Add this component to your project
2. Call with `<toggle-dark-theme />`

# Settings
| Option        | Type          | Default       | Description   |
| ------------- | ------------- | ------------- | ------------- |
| buttons       | Object        | {dark: "Dark mode", light: "Light mode"} | Switch text. For each mode |
| colors        | Object        | {dark: "#0b2137", light": "#ffffff"} | Сolor for each mode. Used in the meta tag `<meta name="theme-color" content="">` |

# Example
`<toggle-dark-theme
      :buttons = '{
          dark: "Enable dark theme",
          light: "Enable light theme"
      }'
      :colors = '{
          dark: "#0b2137",
          light: "#ffffff"
      }'
  />`
