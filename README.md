# colinha

PYCHARM

sudo tar -C /opt/ -xzf Downloads/pycharm-community-2020.3.2.tar.gz
cd /opt/pycharm-community-2020.3.2/bin
sh pycharm.sh

MENU SUPERIOR > Tools > Create Desktop Entry... > OK

Depois busque nos APLICATIVOS e clique com o botão direito e ADICIONAR AOS FAVORITOS

PYTHON - PYENV

sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev git liblzma-dev

curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash

Copie as últimas 3 linhas do comando acima:

Exemplo:
export PATH="/home/junior/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

 E cole no .bashrc e .profile com o comando abaixo:

gedit ~/.bashrc ~/.profile

Feche o terminal e abra novamente!

pyenv update

Veja a ultima versão do Python com o comando abaixo:
pyenv install -l

E instale a ultima versão, como no exemplo abaixo usando a versão 3.9.1.
pyenv install 3.9.1
pyenv global 3.9.1

Ao executar o comando abaixo, a versão que acabamos de baixar, deve conter um asterisco
pyenv versions

CRIANDO PROJETO DJANGO USANDO PIPENV

mkdir nome_do_projeto
cd nome_do_projeto
pip install --upgrade pip pipenv
pipenv --three
pipenv install django
pipenv install python-decouple
pipenv install dj-database-url
pipenv install dj-static
pipenv install django-extensions
pipenv install django-test-without-migrations
pipenv install django-debug-toolbar
pipenv shell
django-admin startproject project .
cd project
mkdir apps
cd ..
django-admin startapp core
Mova todos os apps criados para a pasta "APPS".

python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

python manage.py runserver
