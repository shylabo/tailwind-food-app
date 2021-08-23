# tailwind-food-app

tailwindcss で遊ぶために作ったリポジトリです。
トップページのみ実装しましたが、認証や各種ページへの導線の誘導先ページは実装してません。

This repository is to play with tailwindcss.
I recommend installing tailwind intelliSense which is the extension for tailwindcss.

## npm init

```
$ npm init -y
```

## install tailwindcss

```
npm install tailwindcss
```

## make tailwind.config.js

```
$ npx tailwindcss init --full
```

Notice that if you want to extend tailwindcss property, you can run above without the option "--full" and add some properties to extend field.

## build css

add these scripts and run build command.

```
  "scripts": {
    "build-css": "tailwindcss build -i src/styles.css -o public/styles.css"
  },
```

```
$ npm run build-css
```

Notice that anytime you change something in tailwind.config or styles.css you must run the command.

## custom fonts

If you change the fonts, you can choose font on google fonts and copy the scripts and paste in styles.css.
Add fontFamily field and value ['Nunito'] ,which is a parameter in import url, in tailwind.config.js
e.g.
https://fonts.google.com/specimen/Nunito?query=nunito

```
@import url('https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,200;0,300;0,400;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,600;1,700;1,800;1,900&display=swap');
```

## icons

https://heroicons.com/
