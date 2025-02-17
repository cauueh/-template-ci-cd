# Use uma iamgem official do Python
FROM python:3.10

# Definindo o diretório onde a aplicação será armazenada
WORKDIR /app

# Copiar os arquivos da pasta local para dentro do container
COPY . /app

# Instalar as dependencias de Python de acordo com o que foi desenvolvido na aplicacao e que esta declarado
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Garante que será iniciado a aplicação.
CMD ["gunicorn", "app:app"]