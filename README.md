# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #2 выполнил:
- Гальцов Денис Андреевич
- РИ232702

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | # | 20 |
| Задание 3 | # | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Цель работы
Ознакомиться с основными операторами зыка Python на примере реализации линейной регрессии.

## Задание 1
### Выберите одну из игровых переменных в игре СПАСТИ РТФ Выживание (HP, SP, игровая валюта, здоровье и т.д.), опишите её роль в игре, условия изменения  появления и диапазон допустимых значений. Постройте схему экономической модели в игре и укажите место выбранного ресурса в ней.

Ход работы
В игре Спасти РТФ Выживание сплетено мнного механик, которые вместе образуют геймплей игр жанра аркадный-шутер. Одна из основных механик таких игр - спавн n-ого числа врагов, которых игрок должен убить, чтобы не проиграть. Для того, чтобы игра имела динамику, разработчики добавили магазин оружия и деньги, чтобы со временем у игрока появлялись всё более мощные и сильные орудия убийства. Для поддержания динамики, следует увеличивать как силу игрока, так и силу зомби (внутригрового врага), поэтому динамика игры основана на следующих правилах

- Количество зомби в n-ой волне зависит от уровня игрока и номера конкретной волны
- Урон каждого зомби завист от уровня игрока и номера конретной волны
- У каждого вида зомби есть базовое значение скорости, которое умножается на коэффициент, который завсист от уровня игрока и номера конкретной волны
- В некоторых волнах появляются боссы, но они заменяют собой нескольких зомби (1 босс = 10 обычных зомби)
- Волна представляет собой стек появляющихся зомби, но этот стек разделен в процентном соотнощении на разных представителей зомби и перемешан
(пример 55% - обычные зомби, 35% - лежачие зомби, 10% - зомби боссы)
- На карте может быть ограниченое количество зомби, которое завист от уровня игрока и номера конкресной волны, как только игрок убивает одного из присутствующих на карте, из стека заберается следующий представитель и спавнится на карте
- Из каждого убитого зомби выпадают деньги, игрок может менять количество подбираемых денег за раз при выборе определенных навков навыкам
- В некотрых волнах на игорвой карте появляется сундук под название Аирдроп из которого выпадает валюта игры, количество валюты завсист от уровня игрока и номера конкретной волны, а мест появления сундука выбирается случайно из списка заранее подготовленных мест
- С повышением уровня, игрок может выбрать новый навык иили прокачать старые навыки
- Игрок может покупать оружие и патроны в магазине за валюту, чем силнее оружие - тем оно дороже и тем дороже патроны к оружию

По ссылке ниже прикреплена схема экономической модели игры

[схема экономической модели](https://disk.yandex.ru/i/UzfTelzudU1QfA)

Количество валюты у игрока напрямую связано с динамикой игры, на схеме показано как валюта проявляет себя в игре (как игрок с ней взаимодействует), одноко количество самой валюты - это отражение текущего статуса динамики игры, чем выше динамика - тем больше и быстрее игрок зарабатывает, а также тратит.
Валюту можно тратить на
- патроны
- оружие
Валюта является главным стимулом игрока, так как это объяктивный показатель прогресса в игре (как и игровой уровень), благадаря валюте игра СПАСТИ РТФ ВЫЖИВАНИЕ превращается из простого аркадного шутера в аркадный шутер с элементами прокачки


## Выводы

В ходе данной лабораторной работы, я понял принцип работы экономики как динамического элемента в видеоиграх. Я разобрал экономическую состовляющую игры "Спасти РТФ", благодаря чему смог закрепить свои знания.


| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**