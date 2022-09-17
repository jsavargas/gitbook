# Mkvpropedit

mkvdelspammkvdelspam es un script creado en python por y para el grupo Lat-Team, para la eliminacion del SPAM dentro de las pistas de video/audio/text en los mkv

## Usando Docker <a href="#usando-docker" id="usando-docker"></a>

### mkvdelspam <a href="#mkvdelspam" id="mkvdelspam"></a>

Nos movemos hasta la ruta donde estan los archivos a limpiar y ejecutamos el docker con la instruccion "find ." para que busque todos los archivos y elimine el spam de cada uno de ellosdocker run --rm -it -v "$(pwd):/storage" jsavargas/mkvpropedit:latest find /storage -iname "\*mkv" -exec mkvdelspam {} ;

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi1EvSMy6gwKQw1k9sI54%2Fuploads%2FgE9CvGZKrjOSzBhpaHrn%2Fimage.png?alt=media&#x26;token=a0bc8c93-0f79-4bd8-b394-b31e8cc227b1" alt=""><figcaption></figcaption></figure>

### show-tracks <a href="#show-tracks" id="show-tracks"></a>

​docker run --rm -it -v "$(pwd):/storage" jsavargas/mkvpropedit:latest find /storage -iname "\*mkv" -exec show-tracks {} ;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
