# ZXKM

Предназначен для подключения к Spectrum-совместимым компьютерам, имеющим NemoBUS, HID устройств - 
в часности, USB клавиатуру и мышь. В каждый USB порт можно подключить беспроводную пару клава/мышь, 
либо переходник 2xPS/2->USB. 
Так же могут найти применение другие HID устройства ввода, например графический планшет.

ZXKM успешно работает на следующих компах: Scorpion ZS 256k, Pentagon 128 классика и 2.666, Jasper, Мастер.
**Не использует WAIT.**  
Раскладка клавиатуры и управление дополнительными кнопками может быть изменено при помощи ПО, путём модификации прошивки.  
В исходнике ничего править не надо.

 Сигнал **/DOS** присутствует во всех версиях но не используется. В версии 1.0 он сразу заходит на вывод EPM7128. Подключение к оригинальному ZX, 
 без модификации платы НЕДОПУСТИМО ! 
 В версиях выше 1.0, при необходимости, сигнал **/DOS** подключается перемычкой.
	Сигнал **/Reset** заведён в BUS во всех версиях.

**v1.0** - Должен быть установлен джампер JP1 замыкающий RXD-TXD.  
**v1.0 , v1.1** - управление кнопками Тurbo и Magic выведены на раъем программатора. см. рисунок Magic-Turbo.png  
**v1.1** - Reset, дополнительно выведен на отдельный пин. Добавлен XP2 - для расширения
       функционала (управление какой либо дополнительной кнопкой).
       Сигнал /DOS в текущей прошивке не используется, т.к. Kempston JOY не реализован.  
Добавлены перемычки S0,S1 для дальнейшего развития.  
**v1.4** - Все внешние подключения выведены на дополнительный разъём. Назначение XP1-4 задаются в ПО.  
Добавлены перемычки S0,S1 для дальнейшего развития.

### Клавиатура:
Прошивка "по умолчанию" содержит раскладку всех основных клавиш ZX Spectrum. 
Привязку кнопок ZX к РС клавиатуре можно изменить с помощью прилагаемого ПО.
Так же, на любую РС клавишу можно назначить сочетание двух клавиш ZX. Например - СS+T, SS+P.

В процессе работы, клавиатуру можно запрограммировать на собственные макросы.

Вход в режим программирования:
1. Нажимаем Win+BackSpace - замигал SclollLock.
2. Вводим любые комманды. Макрос ограничен 32-мя клавишами.
   В случае ошибки, жмём ESC и начинаем с пункта 1.
3. После ввода, нажимаем F1-F9. К этой Fх привяжется всё набранное.
Макрос запоминается в энергонезависимой памяти.
  
### Мышь: 

Разрешение(скорость) меняется нажатием **win+1,2,3,4**. Это коэффициент делителя.

**win+0** - инверсия кнопок.

**win+9** - инверсия колеса - **пока не реализовано, В РАБОТЕ.**

Эти настройки запоминаются в энергонезависимой памяти.

### Использование ПО:
**Мануал и видео в работе.**

