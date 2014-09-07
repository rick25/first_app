# Ruby on Rails Tutorial: first application

This is the first application for the
[*Ruby on Rails Tutorial*](http://railstutorial.org/)
by [Ricardo Chinchay].

-Aplicacion creada con :
		rails new first_app

-Luego de modificar el archivo Gemfile :
		bundle install

-Luego inicio un repositorio git en la carpeta del proyecto :
		git init

-Modifico el archivo .gitignore, guardo los cambios y preparo todos los archivos :
		git add .

-Hago el primer commit :
		git commit -m "Repositorio inicial"

-Agrego un repositorio remoto para enviar los cambios a la web :
		git remote add origin https://github.com/rick25/first_app.git

-Mando los datos al repositorio remoto :
		git push -u origin master

-Creo un nuevo brach para poder hacer algunos cambios y me paso a la nueva rama :
		git checkout -b nombre_rama

-Cambio de nombre a un archivo :
		git mv README.rdoc README.md

-Guardo y preparo todas las modificaciones en los archivos bajo seguimiento :
		git commit -a -m "Mejorando el archivo README"

-Ahora cambio a la rama maestra de mi repositorio :
		git checkout master

-Ahora hago una sola las dos ramas (master y nombre_rama)
		git merge master nombre_rama

-Elimino la rama que acabo de unir y que ya no voy a usar :
		git branch -d nombre_rama

-Ahora mando los datos que tengo en el repositorio local al remoto
		git push

