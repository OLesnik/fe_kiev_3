# Домашние задания (Homeworks). GoFrontend#3: Offline
Repository for homeworks "GoFrontend#3: Offline". Mentor: Dmitriy Lisunov

![](http://aws-cf.imdoc.fr/prod/photos/6/4/2/3820642/2844403/img-2844403d28.jpg)

Начиная с **домашнего задания №4** все работы я теперь буду принимать только через `pull requests`.
Общая схема работы изложена здесь: https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project

Есть переводы этой статьи:
- [Українська](https://git-scm.com/book/uk/v2/GitHub-%D0%AF%D0%BA-%D0%B7%D1%80%D0%BE%D0%B1%D0%B8%D1%82%D0%B8-%D0%B2%D0%BD%D0%B5%D1%81%D0%BE%D0%BA-%D0%B4%D0%BE-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D1%83)
- [Русский (переведено не полностью)](https://git-scm.com/book/ru/v2/GitHub-%D0%92%D0%BD%D0%B5%D1%81%D0%B5%D0%BD%D0%B8%D0%B5-%D1%81%D0%BE%D0%B1%D1%81%D1%82%D0%B2%D0%B5%D0%BD%D0%BD%D0%BE%D0%B3%D0%BE-%D0%B2%D0%BA%D0%BB%D0%B0%D0%B4%D0%B0-%D0%B2-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D1%8B)

## Общая схема работы будет выглядеть следующим образом:
1. Делаете `Fork` данного проекта https://github.com/lisunovdv/fe_kiev_3.git как описано в статье
2. Клонируете **СВОЙ** репозиторий `git clone https://github.com/ВАШ_ЛОГИН_GitHub/fe_kiev_3.git` на локальный компьютер
3. Создаёте ветку для домашнего задания (например, для ДЗ №4): `git checkout -b dz_4`
4. Удаляете ненужные файлы документации из master-ветки `git rm -rf .` (если нужно. Можете оставить .gitignore файл)
5. В проекте создаёте **ПАПКУ** с названием `ivanov_i-dz_4` и в ней делаете своё домашнее задание. Название папки должно соответствовать такому *Name Convention* (всё на английском): 

**`Ваша фамилия _ (нижнее подчёркивание) первая буква Вашего имени - (дефис) dz_ номер домашнего задания`**

т.е. как было показано в примере выше, например, вот так `ivanov_i-dz_4`
##### Commit & Push
6. Далее **коммитите и пушите** ветку на GitHub
7. Переходите по адресу `https://github.com/ВАШ_ЛОГИН_GitHub/fe_kiev_3`
8. Выбираете ветку с вашим ДЗ и жмёте `New pull request`

![New pull request](https://github.com/lisunovdv/fe_kiev_3/blob/master/New%20Pull%20Request.jpg)

или, если у Вас появилась кнопка `Compare & pull request`, жмёте её: 
![Compare & pull request](https://git-scm.com/book/en/v2/images/blink-02-pr.png)

## ВАЖНО!!!
9. **Правильно указывайте условия для pull request, иначе GitHub не даст его сделать (НЕ покажет зелёную кнопку ` Create pull request`):**
- 9.1. `base fork:` указываете `lisunovdv/fe_kiev_3`, а `base:` ветку `dz_4` (Для ДЗ № 4 соответственно)
- 9.2. `head fork:` указываете `ВАШ_ЛОГИН_GitHub/fe_kiev_3`, а `compare:` ветку `dz_4` (Для ДЗ № 4 соответственно. Ну или как Вы назвали свою локальную ветку)
- 9.3. После этого жмёте ` Create pull request`
![Правильные настройки pull request](https://github.com/lisunovdv/fe_kiev_3/blob/master/Pull-Request-proccess.jpg)

10. **Заполняете `Title` реквеста в таком формате:** 

`dz_4:ivanov_i:`*Префикс*`:Необязательное короткое сообщение для ментора`

Где *Префикс* может быть:
- **ADD** - Вы только что создали новое ДЗ и ПЕРВЫЙ раз хотите мне его показать
- **CHANGE** - Вы сами обнаружили ошибку и хотите прислать ментору исправленный вариант
- **FIX** - ментор ранее указал Вам на ошибку и Вы высылаете исправленный вариант

11. Если необходимо, можете добавить развёрнутый комментарий в поле ниже:
![Comment](https://github.com/lisunovdv/fe_kiev_3/blob/master/Comment.jpg)

12. После этого жмёте `Create pull request`

13. После этого Ментор принимает решение о принятии ДЗ, либо о его отклонении. Вы можете подписать на уведомления на e-mail о новых комментариях к Вашему ДЗ

## Основная часть обсуждений и комментарии по ДЗ будут здесь, на GitHub, а не в Slack / Facebook
------------------------

# Как добавить старые ДЗ в этот проект?
Например, Вы также хотите добавить Ваши старое ДЗ №2 из другого репозитория.

1. На Вашем локальном компьютере, переходите в папку туда, где у Вас склонирован форк этого проекта `https://github.com/Ваш_Логин_GitHub/fe_kiev_3.git`
2. Добавляете новый внешний источник Вашего старого репозитория со старыми ДЗ под любым именем, отличным от origin, например,  `my_old_repo` вот так:
`git remote add my_old_repo https://github.com/Ваш_Логин_GitHub/OLD_REPO.git`
3. Вытягиваете данные оттуда `git fetch my_old_repo`
4. Создаёте ветку для домашнего задания (например, для ДЗ №2): `git checkout -b dz_2`
5. Удаляете ненужные файлы документации из master-ветки например так: `git rm -rf .`
6. Мёрджите ветку из Вашего старого репозитория `git merge my_old_repo/my_homework_2_old_branch` в текущую `dz_2`
7. Правильно создаёте папку и перемещаете туда файлы Вашего ДЗ ( То есть создаёте **ПАПКУ** с названием `ivanov_i-dz_2` и в неё вставляете своё домашнее задание. Название папки должно соответствовать такому *Name Convention* (всё на английском): **`Ваша фамилия _ (нижнее подчёркивание) первая буква Вашего имени - (дефис) dz_ номер домашнего задания`**, т.е. как было показано в примере выше, например, вот так `ivanov_i-dz_2`
8. После этого можете продолжать с [пункта 6](#commit--push) в начале этого документа
