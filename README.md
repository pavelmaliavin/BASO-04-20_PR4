Сразу извиняюсь за не очень опрятные скрины, скринить неудобно, винда на виртуалке, а лайтшот почему то не работает :)

1) ШИФРОВАНИЕ В WINDOWS. EFS.

Создаем папочку, в папочке создаем текстовик:

<a href="https://ibb.co/y5rkyLG"><img src="https://i.ibb.co/Bj96Z8d/image.png" alt="image" border="0"></a>

Шифруем папку:

<a href="https://ibb.co/ThSC2xz"><img src="https://i.ibb.co/XJgwLrm/image.png" alt="image" border="0"></a>

Готово, папка зашифрована

<a href="https://ibb.co/yRhsnYn"><img src="https://i.ibb.co/JdxkRyR/image.png" alt="image" border="0"></a>

Теперя, создаем новую учетку:

<a href="https://ibb.co/nzNyRJb"><img src="https://i.ibb.co/MMxH90s/image.png" alt="image" border="0"></a>

Заходим через васяна, пытаемся (безуспешно) открыть зашифрованный файл:

<a href="https://ibb.co/yq7R449"><img src="https://i.ibb.co/TtdTWWf/image.png" alt="image" border="0"></a>

Whoops-ie! Не получилось, оно и понятно

Далее будем делать бэкап сертификата ключа шифрования EFS

<a href="https://ibb.co/wpdzKBf"><img src="https://i.ibb.co/TPwgHYs/image.png" alt="image" border="0"></a>

Открываем сертификаты и находим наш, он единственный, потому что один файл и шифровали, логично

<a href="https://ibb.co/wLHtnnQ"><img src="https://i.ibb.co/X4BHnn5/image.png" alt="image" border="0"></a>

Сохраняем и экспортируем, завершая мастер экспорта сертификатов

<a href="https://ibb.co/KK38z0C"><img src="https://i.ibb.co/tLW1Pmy/image.png" alt="image" border="0"></a>

<a href="https://ibb.co/tM39Ybn"><img src="https://i.ibb.co/fYQsrCZ/image.png" alt="image" border="0"></a>

<a href="https://ibb.co/2vfQT2g"><img src="https://i.ibb.co/7n65qc2/image.png" alt="image" border="0"></a>

Все, успешно сохранилось и экспортировалось

Теперь, снова заходим на васяна и пытаемся открыть зашифрованный файл, но перед этим, уже импортируем сертификат на эту учетку

(разрешение скринов поменялось, потому что предыдущий фото-хостинг лег, пришлось сменить, а он почему-то разрешение меняет)

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b40/2011/c9/10745a5f7e29.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b36/2011/86/22e498eff9b3.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b38/2011/2e/e555dbcba737.png" /></a>

И вауля, все открылось, все читается

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b21/2011/b9/2f30321a0f55.png" /></a>

2.CIPHER

Разберемся с шифрованием через консоль

Создаем новый файл для шифрования через консоль (cipher.exe)

<a target="_blank" href="https://radikal.ru"><img src="https://a.radikal.ru/a36/2011/4d/5dfc33fcf120.png" /></a>

Для зашифровки файлов в папке используем комманду cipher /e /s:C:\ciphercmd

<a target="_blank" href="https://radikal.ru"><img src="https://c.radikal.ru/c10/2011/7c/57924d77ec45.png" /></a>

Командой cipher /s:C:\ciphercmd проверяем статус шифровки. Сообщение гласит, что все файлы, которые будут добавленны в папку, автоматически шифроваться не будут

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b03/2011/15/6f0c0b357eb2.png" /></a>

Подробные сведения уже зашифрованной папки можно узнать с помощью комманды cipher /с /s:C:\ciphercmd

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d01/2011/60/565d1396f326.png" /></a>

Командой cipher /x мы можем сохранить бэкапчик сертификата EFS

<a target="_blank" href="https://radikal.ru"><img src="https://c.radikal.ru/c02/2011/ee/8a7044794c43.png" /></a>

Архивация сертификатов EFS успешно завершена!

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d24/2011/03/3369e801b1c7.png" /></a>

Теперь заходим опять в гости к васяну и через другую учетку и начинаем импорт сертификата, а потом открываем сам зашифрованный файл

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b02/2011/88/fcd4261415ce.png" /></a>

Все получилось, точно так же, разницы никакой, между консолью и обычным шифрованием

3.BITLOCKER

Вставляяем флешку с созданным на нем предварительно текстовиком (час я пытался через виртуалку найти эту флешку, ради битлокера:))

<a target="_blank" href="https://radikal.ru"><img src="https://a.radikal.ru/a32/2011/6c/b44700e16001.png" /></a>

Подрубаем битлокер и ждем

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b04/2011/bd/a8a33a3e3d5c.png" /></a>

Ну и все, шифруем 

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d10/2011/1a/18927f43419f.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b21/2011/56/62b803938376.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d39/2011/27/102f1ec99b3c.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://a.radikal.ru/a35/2011/27/a295eb6c5323.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b41/2011/c8/d216f796dfc2.png" /></a>

Шифрование завершенно, вводим пароль и все файлы открылись

<a target="_blank" href="https://radikal.ru"><img src="https://a.radikal.ru/a23/2011/7a/bfd4a80145ba.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d18/2011/4b/0afdf29d7c5d.png" /></a>

4. VERACRYPT

Создадим папку с текстовиком. Откроем веракрипт и создадим том

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b09/2011/59/34919f5ea453.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d24/2011/cc/ca9c1f7adf19.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d39/2011/88/5b2344e268bb.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://c.radikal.ru/c16/2011/6f/13938100a5cc.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b16/2011/1c/0d74d7acc9a9.png" /></a>

Неплохо сделанно с генерацией энтропии через движения мышкой

<a target="_blank" href="https://radikal.ru"><img src="https://c.radikal.ru/c22/2011/00/f8c1c51ae6f2.png" /></a>

Далее просто смонтируем том для нашего файла

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d37/2011/c9/d8397d64c758.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://d.radikal.ru/d23/2011/0b/8a4c51e461ae.png" /></a>

<a target="_blank" href="https://radikal.ru"><img src="https://b.radikal.ru/b34/2011/ed/56d8f687358a.png" /></a>

Смонтировано успешно!

Пароль для прикрепленного файла в репозитории - race1488

сенкс фор вотчин
