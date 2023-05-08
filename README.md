# GIT 

## Содержание
<a href="/pages/1.base.md">Ссылка</a>

## Теория
Три основных секции GIT проекта:
* рабочая копия (the working directory)
* область индексирования (the staging area)
* каталог GIT (GIT directory)
<image src="getImage.png" alt="Основные секции GIT проекта">

Для организации связи между пользователями GIT может использоваться один из следующих протоколов:
* Локальный протокол 
* Умный или тупой HTTP протокол 
* SHH протокол 
* Git протокол 

Локальный протокол это такой способ связи для компьютеров, имеющих одну локальную сеть или вообще только один компьютер. Понятно, что для связи, пользователи должны быть в одной локальной сети. Плюсами данного протокола являются простота взаимодействия и простота настройки. Минусы - невозможность работы удаленно от этой сети, риск потери данных (особенно если это один компьютер).  

Протокол HTTP изначально использовался только для чтения, позже с приходом умного протокола, сам использоваться и для записи. По всем атрибутам схож с SSH протоколом, но у него более простой способ коммуникации. Нет аутентификации.   

SHH протокол более защищённый, у него есть аутентификация. Он лучше сжимает данные и он настроен по дефолту в системах Linux. Но даже если он не настроен то это не беда - ведь это протокол с которым знакомы многие системные администраторы. 

GIT протокол является самым сложным из всех. Сложность настройки, более сложный доступ к репозиториям. 

В качестве удаленных репозиториев самым оптимальным является использование GIT хостингов, таких как GitLab, GitHub и так далее. Удаленный репозиторий является оптимальным для использования как в личных проектах, так и в работе в команде.  

В качестве распределенной работы могут быть применены несколько скриптов работы с git.  

Например метод, когда есть один администратор, который сливает ветки в свою ветку мастер. Или метод работы, когда есть несколько администраторов, у каждого из которых есть свои «лейтенанты», которые в первую очередь собирают данные от разработчиков и сливают их ветки со своими. А администраторы работают только с ветками «лейтенантов».  

Каждый метод по своему хорош и используется в зависимости от объёма и размеров системы. Одно дело работать с мелким проектом, другое дело - с ядром LINUX.