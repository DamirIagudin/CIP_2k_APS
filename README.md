В папке ПО:
Панель оператора:
Файл CIP_2k.emcp - это сжатый файл проекта. В нем всё должно быть - элементы из используемых библиотек и проч. Чтобы восстановить из него файл проекта (с раширением .emtp) используем File - Compress/Uncompress. Так что если я буду отправлять тебе проект можешь использовать этот файл в случае ссылок на другие библиотеки.
Файл CIP_2k.emtp - это основной файл проекта, исходник.
Файл CIP_2k.exob - это скомпиллированный файл, который загружается в панель оператора.
Recipe_CIPwork.rcp - это файл рецептов, в нашем случае в рецептах хранятся настройки маршрутов (объектов мойки). Для редактирования и создания рецептов использовал Utility Manager - Data Conversion - Recipe Editor (по рецептам потом подробнее могу рассказать).
Контроллер:
CIP_2k.pro - файл проекта для CoDeSys.
My_lib.lib - моя библиотека, используемая в проекте. Чтобы проект у тебя компиллировался эту библиотеку нужно в Менеджере библиотек (в CoDeSys) добавить, указав ее реальное место расположение на твоем диске. У меня она лежит здесь:  C:\Program Files (x86)\WAGO Software\CODESYS V2.3\Library . Если сюда положишь не надо будет каждый раз ее добавлять.
Остальные это служебные файлы CoDeSys.


Установочное ПО (ссылка отдельно):
CODESYS_2.3.9.61_RELEASE_BUILD_20200326.zip  - дистрибьютив CoDeSys версии 2.3.9.61 (Build Oct 22 2019). Это CoDeSys для контроллеров Wago со всеми необходимыми таргетами контроллеров.
WAGO_EthernetSettings_Setup_v6.8.2.2_full.exe  - утиллита для настройки и параметрирования ПЛК, в частности использую для настройки сетевых адресов. Работает как по Ethernet, так и по Serial через специальный переходник от USB (переходник должен быть у Щелыканцева, подключать при ВЫКЛЮЧЕННОМ ПЛК!). Пр настройке адресов потом могу отдельно рассказать.
WAGO_IOCheck3_Setup_v3.15.3(01)_full.exe  - утилита для диагностики ПЛК, параметрирования отдельных модулей расширения (которые поддерживают параметрирование), а также для принудительного управления выходами ПЛК.


16.02.23г.
Добавлена папка ТЗ. В ней схема функциональная, спецификация оборудования, описание.

17.02.23г.
Добавлена папка Оборудование ДОК. В ней будут размещаться мануалы и документация по отдельным единицам оборудования, входящего в проект. Например документация по ПЛК, панели оператора, частотным преобразователям и проч. 

07.03.23г.
Добавлен файл "Настройки частотников" в папку Оборудование ДОК