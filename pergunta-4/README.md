# Enunciado da Questão
    Pergunta 4 — Containers (Docker)
        Gerenciamos ambientes usando containers e queremos ver isso na prática, de forma simples.
        Parte teórica (no README):
        
# Qual a vantagem de usar containers em vez de configurar tudo manualmente no servidor?
Resposta: O docker permite que a aplicação seja a mesma, independênte de onde estiver sendo provisionada, isso é feito quando uma imagem é gerada a partir do repositório da aplicação, cada imagem tem a sua versão o que facilida na hora de fazer o deploy e rollbacks. Com as imagens podemos ter vários containers rodando dentro do mesmo servidor, por exemplo, nginx, Postgres, Grafana, etc. cada um com o seu próprio container. Além que o arquivo docker compose pode conter environments, portas, volumes, container_name e commands pré-configurados. Assim podemos usar o comando docker compose up para subir os containers rapidamente, e docker compose down para derrubá-los.  

# O que significa idempotência nesse contexto? O que acontece se docker compose up rodar duas vezes num ambiente já configurado?



## Entrega de código:
    Escreva um docker-compose.yml que suba Nginx + PHP-FPM + MariaDB para um ambiente
    de desenvolvimento local. O Nginx deve servir um index.php com phpinfo() , e os dados do
    MariaDB devem persistir entre restarts via volume.

