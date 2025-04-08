# Learn Docker Compose

Botando em prática os estudos de Docker Compose, foi criado um *compose* com API e frontend rodando simultaneamente.

## Subindo o Compose

Resultado dos comandos rodados para subir o projeto:

```bash
davi.candido@D1320:~/Documentos/Alura/DevOps/alurabooks$ sudo docker compose up -d
WARN[0000] /home/davi.candido/Documentos/Alura/DevOps/alurabooks/docker-compose.yml: the attribute `version` is obsolete, it will be ignored, please remove it to avoid potential confusion 
[+] Running 3/3
 ✔ Network alurabooks_default       Created                                                                                          0.1s 
 ✔ Container alurabooks-frontend-1  Started                                                                                          9.5s 
 ✔ Container alurabooks-backend-1   Started                                                                                          9.5s 
```

## Verificando containers em execução

```bash
davi.candido@D1320:~/Documentos/Alura/DevOps/alurabooks$ sudo docker ps -a
CONTAINER ID   IMAGE              COMMAND                  CREATED          STATUS         PORTS                                         NAMES
5e02e326ae6e   front-alurabooks   "docker-entrypoint.s…"   15 seconds ago   Up 5 seconds   0.0.0.0:3000->3000/tcp, [::]:3000->3000/tcp   alurabooks-frontend-1
e134ac5c3535   api-alurabooks     "docker-entrypoint.s…"   15 seconds ago   Up 5 seconds   0.0.0.0:8000->8000/tcp, [::]:8000->8000/tcp   alurabooks-backend-1
```

## Demonstração

Abaixo, vídeo demonstrativo do funcionamento do site utilizado:

📹 **[Clique aqui para assistir ao vídeo](./midia/demo.webm)**

## Créditos

Projeto criado usando um projeto de API e Front-end público da **Alura**.
