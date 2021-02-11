
% prepara el repositorio para su despliegue. 
release: RUN python3 ./manage.py collecstatic
	 sh -c 'cd decide && python manage.py migrate'
% especifica el comando para lanzar Decide
web: sh -c 'cd decide && gunicorn decide.wsgi --log-file -'