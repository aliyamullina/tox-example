# Tox
#### Установка зависимостей
```
pip install -r requirements.txt
```
#### Запуск tox
```
tox
```
#### Запуск [testenv:linters]
```
tox -e linters
```
# Git
#### Создать `hey` на основе текущей `main`
```
git checkout -b hey main
```
#### Залить локальную `hey` на удаленную `origin/hey`
```
git push origin hey
```
#### Слияние `hey` в `main`
```
git checkout main
git merge hey
```
#### Подтянуть изменения из `main` в `hey`
Получаю последние изменения
```
git checkout main
git pull
```
Перехожу в свою ветку
```
git checkout hey
```
Если надо hey поверх main, то
```
git rebase main
```
Если объединить,то
```
git merge main
```
#### Отменить изменения в `requirements.txt`
```
git checkout requirements.txt
```
#### Перезапись истории в трех последних коммитах, работа с [VIM](#VIM)
```
git rebase -i HEAD~3
git push --force
```
#### Сбросить до коммита и отправить изменения
```
git log
git reset --hard a3775a5485af0af20375cedf46112db5f813322a 
git push --force
```
#### Создать ветку `hey` от коммита из ветки `main`
```
git checkout ffb2e33dc0ecae5f2a917e666f6b3ed602ac2025
git switch -c hey
git push origin hey
```

# VIM
#### Начать режим редактирования
Нажать `i`
```
r - изменить только текст коммита
```
#### Выход
Нажать `Esc`
```
:wq
```
# Screen Mac
#### Окно
```
cmd + shift + 3
```
#### Область
```
cmd + shift + 4
```
# Github CI/CD, github actions
#### Добавить в корень проекта
```
.github/workflows/tests_ci.yml
```
#### Документация
[docs.github.com/en/actions](https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#jobsjob_idsteps)

# conftest.py
#### Полноэкранный режим
```
add_options.add_argument("--start-fullscreen")
```
#### Запуск без отображения браузера
```
add_options.add_argument("--headless")
```
