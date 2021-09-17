# WebBox
Чтобы запустить на lighttpd
Скачайте и установите lighttpd <p>
```sh
  sudo apt install lighttpd
```

Далее создайте конфигурационный файл для запуска сервера
```
server.document-root = "<Здесь путь до корневой папки проекта>"

server.port = <порт> 

server.username = "www"
server.groupname = "www"

mimetype.assign = (
  ".html" => "text/html",
  ".js" => "text/javascript",
  ".css" => "text/css",
  ".txt" => "text/plain",
  ".jpg" => "image/jpeg",
  ".png" => "image/png",
  ".fbx" => "text/plain"
)

index-file.names = ("index.html")
```

Теперь чтобы запустить lighttpd
```sh
lighttpd -f <путь до конфигурационного файла>
```

удачи :)
Если у вас винда, разбирайтесь сами. Делюсь опытом исключительно для убунтистов и других линуксоидов.

Ссылки на документацию lighttpd найдете
