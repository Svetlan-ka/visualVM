```java
(1) Please open 'ru.netology.JvmExperience' in VisualVm
(2) 13:57:14.867997700: loading io.vertx
(3) 13:57:16.161983: loaded 529 classes
(4) 13:57:19.185887100: loading io.netty
(5) 13:57:21.583429100: loaded 2117 classes
(6) 13:57:24.588582: loading org.springframework
(7) 13:57:25.439302800: loaded 869 classes
(8) 13:57:28.447156400: now see heap
(9) 13:57:28.448032700: creating 5000000 objects
(10) 13:57:29.252794: created
(11) 13:57:32.268676900: creating 5000000 objects
(12) 13:57:32.955959900: created
(13) 13:57:36.096857700: creating 5000000 objects
(14) 13:57:36.865177100: created

```
***
![metaspace](https://github.com/Svetlan-ka/visualVM/blob/main/metaspace.png?raw=true)

На графике представлена загрузка системных и программно указанных классов для работы программы. 

***
![classes](https://github.com/Svetlan-ka/visualVM/blob/main/classes.png?raw=true)

На графике представлена выгрузка классов из указанных в запросе пакетов.


***
![heap](https://github.com/Svetlan-ka/visualVM/blob/main/heap.png?raw=true)

(2, 4, 6): создание объектов _reflections_ в методе _loadToMetaspaceAllFrom_. \
(9-14): создание новых объектов в методе _createSimpleObjects_.

