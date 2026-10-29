# Lurker theme for thelounge

Monokai Plus theme based on <a href="https://github.com/amiantos/lurker">Lurker's default theme</a>

<a href="https://yarn.pm/thelounge-theme-lurker"><img alt="npm version" src="https://img.shields.io/npm/v/thelounge-theme-lurker.svg?style=flat-square"></a>
<a href="https://npm-stat.com/charts.html?package=thelounge-theme-lurker&from=2016-02-12"><img alt="Total downloads on npm" src="https://img.shields.io/npm/dt/thelounge-theme-lurker.svg?colorB=007dc7&style=flat-square"></a>

### Install using thelounge

```bash
thelounge install thelounge-theme-lurker
```

### Upgrade using thelounge

```bash
thelounge upgrade thelounge-theme-lurker
```

### Customizing Theme

You can add these snippets on your custom stylesheet.

#### Use JetBrains Mono font

The following code will use JetBrains Mono, will fall back to Input and monospace, in an ascending order of font's availability.

```css
@import url("https://fonts.googleapis.com/css?family=JetBrains+Mono&display=swap");

* {
 font-family: 'JetBrains Mono', 'Input', monospace;
}
```

#### User list customization

If you want to make the user tab look more like Lurker, you can use the following CSS code.

This removes permission-wise tabs from the user list

```css
#chat .user-mode::before {
  display: none;
}

#chat .user-mode {
  margin-top: 0;
  margin-bottom: 0;
}

#chat .user-mode.normal .user {
  padding-left: 10px;
}
```

This removes the user search bar.

```css
#chat .userlist .count {
    display: none;
}
```

This removes the user status.
```css
#chat .user-mode .status-icon {
  display: none;
}

#chat .user-mode.normal .user {
    padding-left: 19px;
}
```