# eleicoes_2022
Dados das Eleicoes Capturados do TSE

# Download dos Dumps em Mysql

# 1o Turno
https://1drv.ms/u/s!AjY3aBdCKABKj5Jh2iExxl83eedGCQ

# 2o Turno
https://1drv.ms/u/s!AjY3aBdCKABKj5Jg-Dt0x-EslF93Ng


# Para o docker compose
# No WSL ou Linux
sudo apt-get install docker
sudo apt-get install docker-compose
sudo /etc/init.d/docker start

# Copiar o arquivo docker-compose.yml
sudo docker-compose up

# A senha do arquivo : joao1633

# Descompactar o Dump
unzip vota22_2.zip

# Para importar o dump no mysql do docker-compose
sudo cat vota22_2.sql | sudo docker exec -i mysql_db_1 /usr/bin/mysql -u root --password=password eleicoes
