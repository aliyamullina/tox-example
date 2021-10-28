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
#### Создать ветку cake на основе текущей main
```
git checkout -b cake main
```
#### Слияние hey в main
```
git checkout main
git merge hey
```
#### Подтянуть изменения из main в hey
```
git checkout hey
git rebase main
```
#### Отменить изменения в файле requirements.txt
```
git checkout requirements.txt
```
#### Перезапись истории в трех последних коммитах
```
git rebase -i HEAD~3
```
#### Сбросить до коммита
```
git reset --hard a3775a5485af0af20375cedf46112db5f813322a 
git push --force
```

# VIM
#### Начать режим редактирования
Нажать `i`
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
