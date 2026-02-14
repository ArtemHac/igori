# Как выложить проект на GitHub

## 1. Создайте репозиторий на GitHub

1. Зайдите на [github.com](https://github.com) и войдите в аккаунт.
2. Нажмите **"+"** → **"New repository"**.
3. Укажите имя репозитория (например, **igori**).
4. Выберите **Public**.
5. **Не** ставьте галочки "Add a README" и "Add .gitignore" — репозиторий должен быть пустым.
6. Нажмите **"Create repository"**.

## 2. Подключите репозиторий и отправьте код

В папке проекта выполните в терминале (подставьте **ВАШ_ЛОГИН** и **ИМЯ_РЕПО**):

```bash
git remote add origin https://github.com/ВАШ_ЛОГИН/ИМЯ_РЕПО.git
git branch -M main
git push -u origin main
```

Пример, если логин `artem` и репозиторий `igori`:

```bash
git remote add origin https://github.com/artem/igori.git
git branch -M main
git push -u origin main
```

## 3. Включите GitHub Pages (чтобы лендинг открывался по ссылке)

1. В репозитории на GitHub: **Settings** → **Pages**.
2. В разделе **Source** выберите **Deploy from a branch**.
3. В **Branch** выберите **main** и папку **/ (root)**.
4. Сохраните (**Save**).

Через пару минут сайт будет доступен по адресу:
`https://ВАШ_ЛОГИН.github.io/ИМЯ_РЕПО/`

Например: `https://artem.github.io/igori/`
