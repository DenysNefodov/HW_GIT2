# HW_GIT2

* На локальном репозитории сделать ветки для:
    * Postman
    * Jmeter
    * CheckLists
    * Bag Reports
    * SQL
    * Charles
    * Mobile testing
```Bash
git branch Postman
git branch Jmeter
git branch CheckLists
git branch BugReports
git branch SQL
git branch Charles
git branch MobileTesting
```

**Запушить все ветки на внешний репозиторий**
```Bash
git push -u origin Postman
git push -u origin Jmeter
git push -u origin CheckLists
git push -u origin BugReports
git push -u origin SQL
git push -u origin Charles
git push -u origin MobileTesting
```
**В ветке Bag Reports сделать текстовый документ со структурой баг репорта**
```Bash
git checkout BugReports
touch bug_reports.txt
```
```TXT
ID - Уникальный идентификационный номер
Summary/Title - Что? Где? Когда?
STR - Шаги воспроизведения
Actual Result - Фактический результат
Expected Result - Ожидаемый результат
Environment - Окружение
Project - Название проекта
Module - Компонент/модуль/юнит, в котором обнаружен дефект
Build - Версия сборки
Severity - Критичность бага по степени влияния на продукт
Priority - Критичность бага по степени влияния на бизнес
Status - Статус бага в жизненном цикле бага
Author - Тот, кто нашёл баг
Assigned to - Назначен
Attachments - Логи/скриншоты/видео
```
**Запушить структуру багрепорта на внешний репозиторий**
```Bash
git add .
git commit -m "add structure bugreports in file bug_reports.txt"
git push -u origin BugReports
```
**Вмержить ветку BugReports в Main**
```Bash
git merge BugReports
```
**Запушить main на внешний репозиторий.**
```Bash
git push
```
**В ветке CheckLists набросать структуру чек листа.**
```Bash
git checkout CheckLists
cat >> checklist.txt
```
```TXT
ID
Summary
Section
Enviroment
Expected Result
Status
Bug report link
```
**Запушить структуру на внешний репозиторий**
```Bash
git add .
git commit -m "add structure checklist in file checklist.txt"
git push -u origin CheckLists
```
**На внешнем репозитории сделать Pull Request ветки CheckLists в main**
```Bash
Нажать кнопку "Compare & pull request"
Нажать "Create pull request"
После проверки нажать "Merge pull request"
Нажать "Confirm merge"
После слияния веток должно быть указано Pull request successfull merged and closed.
```
**Синхронизировать Внешнюю и Локальную ветки Main**
```Bash
git checkout main
git pull https://github.com/DenysNefodov/HW_GIT2.git
git push
```
