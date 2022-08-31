# Notice
## Конспект по изучению Git

git clone https://github.com/libgit2/libgit2 клонироует репозиторий (на локальный диск)

 git clone https://github.com/libgit2/libgit2 mylibgit
Эта команда делает всё то же самое, что и предыдущая, только результирующий каталог будет назван mylibgit.

git status - Основной инструмент, используемый для определения, какие файлы в каком состоянии находятся 


## Создать новый репозиторий или проект

```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/LeonidUspeshny/test.git
git push -u origin main
```

Отслеживание новых файлов git add README

Если вы изменили файл после выполнения git add, вам придётся снова выполнить git add, чтобы проиндексировать последнюю версию файла:

```
ы можете создать файл .gitignore. с перечислением шаблонов соответствующих таким файлам. Вот пример файла .gitignore:

$ cat .gitignore
*.[oa]
```

Вы можете набрать свой комментарий к коммиту в командной строке вместе с командой commit указав его после параметра -m, как в следующем примере:
$ git commit -m "Story 182: fix benchmarks for speed"

```
Добавление параметра -a в команду git commit заставляет Git автоматически индексировать каждый уже отслеживаемый на момент коммита файл, позволяя вам обойтись без git add:
```
