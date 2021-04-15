Criar ambiente virtual 
 ````
 python -m  venv nomeDoAmbiente 

 conda create --name nomeDoAmbiente python =3.8 // conda
````
Ativando o ambiente
````
nomeDoAmbiente\scripts\activate 

conda activate nomeDoAmbiente
````
Instalar as dependencias
````
pip install nomdeDaDependecia
pip install requirements.txt // qdo vc tiver uma arquivo com os nomes das dependencias
````
Criando o projeto
````
django-admin startproject nomeDoProjeto . 
````
Rodando o servidor
````
python .\manage.py runserver
python manage.py runserver 
````
Executando o docker
````
docker-compose up --build
````
rodando o docker
````
docker-compose up -d  // esse aqui é pra vc deixar rodando o docker sem precisar abrir um novo terminal
````
se quiser ficar vendo os logs do docker
````
docker-compose up -d
````
Criar o app user temos 3 formas de fazer 
````
docker-compose exec web python manage.py start app users 

manage.py start app users 

docker-compose exec bash

````
rodar o teste
````
docker-compose exec web pytest
````
rodar o teste
````
docker-compose exec web pytest
````
rodar o teste 2
````
docker-compose exec web pytest --cov --cov-report=html
````
makemigrations
````
docker-compose exec web python manage.py makemigrations
````
migrate
````
docker-compose exec web python manage.py migrate
````
teste de usuario
````
docker-compose exec web web pytest -x  #se ele encontrar qualquer erro ele para
````
Criando super user
````
docker-compose exec web web python manage.py createsuperuser
````
Iniciando o app
````
docker-compose exec web web python manage.py startapp pages
````
teste com cobertura, ele mostra o quanto foi coberto 
````
docker-compose exec web web pytest -x  --cov 
````
Importanto um json pro bd
````
docker-compose exec web web python manage.py loaddata nomeDoJason
````






dependencia | Descrição ||
------ | ------- | ---------:
**django==3.1.3**|Django em si  | 
**django-autoslug==1.9.8**| preenchimento automático |
**django-debug-toolbar==3.1.1** | ferramenta para debugar o request e response da aplicação.|
**django-model-utils==4.1.0** | models no Django, cria colunas para dizer quando foi criado e alterado o objeto.|
**factory-boy==3.1.0**| cria produtos e categorias
**ipython==7.19.0**|para melhorar o uso shell
**pillow==8.0.1**| trabalha com imagens
**psycopg2==2.8.6**| postgree sql
**pytest==6.1.2**| testes 
**pytest-cov==2.10.1**| testes 
**pytest-django==4.1.0**|testes 


