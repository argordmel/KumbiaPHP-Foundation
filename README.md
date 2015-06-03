# KumbiaPHP, Foundation With Sass & LiveReload

[KumbiaPHP](http://kumbiaphp.com/)
[Foundation](http://foundation.zurb.com/docs/)
[Sass](http://sass-lang.com/guide)
[LiveReload](http://livereload.com/)

## Instalación en ubuntu o mac

####Instalando elementos necesarios
`sudo apt-get install build-essential g++ (Esto no en mac)`


####Instalando Ruby (Comprobar si ya está instalado)
`sudo apt-get install ruby1.9.1 ruby1.9.1-dev (Eso no en mac)`


####Instalando LiveReload y compresión de archivos
`sudo gem install bundle guard guard-livereload jsmin cssmin`


####Instalando LiveReload y compresión de archivos
`sudo gem install bundle guard guard-livereload jsmin cssmin`


####Desinstalando Sass y Compass
`sudo gem uninstall sass`

`sudo gem uninstall compass`


####Instalando Sass y Compass
`sudo gem install sass --version 3.2.19`

`sudo gem install compass --version 0.12.2`


####Verificando dependencias para el LiveReload (Solo se ejecuta una sola vez)
Dentro del proyecto (en el root folder):

`bundle install`


####Activando el LiveReload
Dentro del proyecto (en el root folder):

`bundle exec guard`


####Activando el compilador para el Sass
Dentro de la carpeta public:

`compass watch`


####Instalando extensión en el navegador
[Extensiones](http://livereload.com/extensions/)



####Creando Alias para los comandos
Dentro la carpeta personal ~:

`nano .bash_profile`

Agregarmos los alias respectivos

`alias LiveReload='bundle exec guard'`

`alias CompassWatch='compass watch'`

Guardamos (ctrl + o y ctrl + x)

`source .bash_profile`
