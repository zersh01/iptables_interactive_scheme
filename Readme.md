Support lang:
- [Русский](#Rus)
- [English](#En)

# Rus 
## Интерактивное описание таблиц iptables.

Demo: https://zersh01.github.io/iptables_interactive_scheme/

Основные файлы:

- iptables.html - разметка
- styles.css - стили
- iptables.svg - непосредственно схема
- Iptables - папка для локализаций
- start_python_http.sh - простой http сервер для быстрого тестирования

Пример:
![alt text](https://github.com/zersh01/iptables_interactive_scheme/raw/main/iptables_example.gif "iptables")


Вы можете прислать свою локализацию, добавив  перевод по следующему пути: Iptables/lang_name

Файлы: 

*-data - для всплывающих подсказок

*-descr - расширенное описание под схемой

extensions/ - каталог для локализации [iptables-extensions](https://ipset.netfilter.org/iptables-extensions.man.html)

Файлы в extensions должны именоваться следующим образом: 

*имя  + '_' + 'имя таблиц' (или цепочки)*  - в которых данное расширение должно использоваться.

Например следующее имя создаст пункт DNAT и подсвечивает таблицы nat в цепочках PREROUTING и OUTPUT:

```bash 
DNAT_prerouting-nat_output-nat
```
Следующий пример создаст пункт REJECTv4 и подсветит соответствующие цепочки:

```bash 
REJECTv4_input_forward_output
```

Источник схемы: https://commons.wikimedia.org/wiki/File:Iptables_diagram.png

# En

## Interactive description of iptables tables.

Demo: https://zersh01.github.io/iptables_interactive_scheme/

Basic files:

- iptables.html - markup
- styles.css styles
- iptables.svg - the schema itself
- Iptables - folder for localizations
- start_python_http.sh - simple http server for quick testing

You can send your localization by adding a translation along the following path: Iptables/lang_name

The file names indicate the type of message that they are intended for:

*-data - for tooltips

*-descr - extended description under the diagram

extensions/ directory is for localization of [iptables-extensions](https://ipset.netfilter.org/iptables-extensions.man.html).

Files in the extensions directory should be named as follows:

*name + '_' + 'name of tables' (or chains)* - in which this extension should be used.

For example, the following name will create an entry for DNAT and highlight the nat tables in the PREROUTING and OUTPUT chains:
```bash
DNAT_prerouting-nat_output-nat
```
The next example will create an entry for REJECTv4 and highlight the corresponding chains:
```bash
REJECTv4_input_forward_output
```
