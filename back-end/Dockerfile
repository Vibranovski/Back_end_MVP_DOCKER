# Use uma imagem Python 3.11
FROM python:3.11-slim

# Define o diretório de trabalho dentro do container
WORKDIR /app

# Instala curl para healthcheck
RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*

# Copia os arquivos da aplicação para o container
COPY back_end.py .
COPY requirements.txt .

# Instala as dependências Python
RUN pip install --no-cache-dir -r requirements.txt

# Expõe a porta 5000
EXPOSE 5000

# Define variáveis de ambiente
ENV FLASK_APP=back_end.py
ENV FLASK_ENV=development

# Comando para iniciar a aplicação
# Vincula em 0.0.0.0 para aceitar conexões de fora do container
CMD ["python", "back_end.py"]
