# Сергей Абрамов - «Системы контроля версий»

---

## Решение

### Создание репозитория и первого коммита

1. Зарегистрировал аккаунт на (https://github.com/) и создал репозиторий devops-netology.

![git1](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git1.jpg)

2. Я создал SSH-key , т.к. при таком варианте нет необходимости постоянно вводить пароль и работаю я только со своей виртуальной машины. И склонировал репозиторий.

![git2](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git2.jpg)

3. Произвел первоначальную настроику.

![git3](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git3.jpg)

4. Выполните команду git status и запомните результат. Отредактируйте файл README.md любым удобным способом, тем самым переведя файл в состояние Modified.

![git4](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git4.jpg)

5. Команда git diff отображает информацию о файле и что он еще в состоянии modified.
Команда git diff --staged отображает эту же информацию , но уже когда фаил перешел в сотояние staged.

![git5](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git5.jpg)

6. Сделал коммит, посмотрел выводы команд git status, git diff и git diff --staged.

![git6](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git6.jpg)

### Создание файлов .gitignore и второго коммита

1. Создал файл .gitignore. Добавил файл .gitignore в следующий коммит (git add...).

![git7](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git7.jpg)

2. Создал каталог terraform и внутри этого каталога — файл .gitignore.

![git8](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git8.jpg)

### Описание своими словами, что игнорируется:

**/.terraform/* - все скрытые файлы .terraform , во всех коталогах с этим именем.

*.tfstate - все файлы с расширением tfstate в корне.

*.tfstate.* - все файлы имеющие в имени  любое колличество символов. tfstate (эти симолы) .любое колличество символов
crash.log - данный лог файл

crash.*.log - данное имя . любое колличество символов .log 

*.tfvars - все файлы с расширением fvars в корне.

*.tfvars.json - любое колличество символов .tfvars.json

override.tf
override.tf.json - два этих фаила в корне.

*_override.tf
*_override.tf.json - любое колличество символов и эти два окончания

.terraformrc
terraform.rc - два фаила с такими именами


3. Закоммител результат работы с комментарием Moved and deleted.

![git9](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git9.jpg)

### Проверка изменения

![git10](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git10.jpg)

### Отправка изменений в репозиторий

![git11](https://github.com/smabramov/Version-control-systems/blob/ce6a899620aab0f9a2e04e78358e17ac3c89ca37/jpg/git11.jpg)



