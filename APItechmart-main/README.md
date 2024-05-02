#Siga os comandos abaixo no terminal:

python -m venv venv

cd venv/Scripts

activate



pip install mysqlclient

cd api-main

pip install django

pip install djangorestframework



python manage.py makemigrations

python manage.py migrate

python manage.py createsuperuser

python manage.py runserver




No Xampp, ativar MySQL e Apache

Abrir terminal e digitar o comando mysql -u root -p

CREATE DATABASE produtos;

USE produtos;

CREATE TABLE produtos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome_do_produto VARCHAR(255),
    detalhes TEXT,
    estoque INT,
    preco DECIMAL(10, 2)
);

