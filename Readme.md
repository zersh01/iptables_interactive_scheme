Support lang:
- [Русский](#Rus)
- [English](#En)
- [Chinese](#zh_CN)

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

# zh_CN

## iptables 的交互式描述

演示: https://zersh01.github.io/iptables_interactive_scheme/

基本文件:

- iptables.html - 主页
- styles.css - 样式
- iptables.svg - 图表
- Iptables - 语言文件夹
- start_python_http.sh - 用于快速测试的简单 HTTP 服务器

您可以通过在以下路径添加翻译来发送您的本地化：Iptables/lang_name

文件名指示它们所针对的消息类型：

*-data - 用于工具提示

*-descr - 图表下的扩展描述

extensions/ 目录用于 [iptables-extensions](https://ipset.netfilter.org/iptables-extensions.man.html) 的本地化。

extensions 目录中的文件应按以下方式命名：

*name + '_' + '表名'（或链名）* - 在此扩展应使用的表（或链）中。

例如，以下名称将为 DNAT 创建一个条目，并在 PREROUTING 和 OUTPUT 链中突出显示 nat 表：
```
DNAT_prerouting-nat_output-nat
```
下一个示例将为 REJECTv4 创建一个条目，并突出显示相应的链：
```
REJECTv4_input_forward_output
```
