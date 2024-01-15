# ДЗ полезные советы

### Ошибки линтера: 

Часть ошибок лечится простой командой: 

```
golangci-lint run --fix
```

Ошибка линтера 
```go
level=error msg="[linters_context] gocritic: load embedded ruleguard rules: rules/rules.go:13: can't load fmt: setting an explicit GOROOT can fix this problem."
```
обычно означает что версия линтера не совпадает с версией go. Лечится изменением версии линтера до последней в `.github/workflows/` папке. 

### Задания:

Во всех заданиях есть файл `go.mod` в котором изначально прописаны только шаблоны путей до ваших модулей ДЗ (так как у каждого будет свой путь к репе). 
Все их можно найти поискав `fixme_my_friend` по файлам. Пути к модулю форумируются из имени репы и вашего логина. Не
забывайте изменить их под ваш репозиторий. 
Как вариант можно разделаться с этим раз и навсегда сразу поправив пути как они должны быть. 


#### Тесты 
В каждом задании, для получения проходного балла, за исключением первого должен быть написан хотя бы 1 новый тест.
Не возбраняется писать больше тестов, естественно. 


#### .sync файлы
Это файлы маркеры которые используются гит actions для обновления папок в которых они расположены в случае изменений в основном репозитории.
Если вы не хотите чтобы ваши изменения перетирались при внесении изменений в основное репо к примеру, то файлы `.sync` желательно удалить. 

#### ДЗ Календарь 
Является самым объемным по коду, и предшествует проекту, 
для упрощения его проверки, рекомендую заранее обновлять readme файл с 
описанием как запускать ваше решение, и какие из портов и эндпойнтов готовы.
Можно под это дело создать и коллекцию постмена и сложить в тот же репозиторий.

#### ДЗ Проект
Рекомендую делать в отдельном репозитории, и сдавать пошагово, как и календарь, 
для упрощения его проверки. Все вышеперечисленные советы по календарю так же применимы и к проекту.

