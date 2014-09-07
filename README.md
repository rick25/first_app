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

-Modificamos el Gemfile para poder usar Heroku :
		source 'https://rubygems.org'
		ruby '2.1.2'	#agregado

		gem 'rails', '4.1.5'	#4.0.8
		group :development do
			gem 'sqlite3'			#1.3.8
		end
		gem 'sass-rails', '4.0.3'	#ok
		gem 'uglifier', '2.1.1'		#2.1.1
		gem 'coffee-rails', '4.0.0'	#4.0.1
		# gem 'therubyracer',  platforms: :ruby

		gem 'jquery-rails', '3.0.4'		#3.0.4
		gem 'turbolinks', '1.1.1'		#1.1.1
		gem 'jbuilder', '2.0'	#1.0.2

		group :doc do
			gem 'sdoc', '0.3.20', require: false	#0.3.20
		end
		group :production do
			gem 'pg', '0.15.1'
			gem 'rails_12factor', '0.0.2'
		end
		#gem 'spring',        group: :development

-Hago :
		bundle install --without production

-Hago otra confirmacion :
		git commit -a -m "Actualizado gemfile.lock para Heroku" 

-Me logueo en Heroku :
		heroku login

-Dentro de la carpeta del proyecto hacemos :
		heroku create

-Mando el repositorio a heroku :
		git push heroku master

-Para poder ver la aplicacion en heroku :
		heroku open

-Ahora mando los datos que tengo en el repositorio local al remoto
		git push