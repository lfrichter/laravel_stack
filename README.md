<p align="center"><img src="https://res.cloudinary.com/dtfbvvkyp/image/upload/v1566331377/laravel-logolockup-cmyk-red.svg" width="400"></p>

---

## Desafio 1

Baseado em nosso projeto exemplo Laravel, utilize o sistema de templates do Dockerize para que ele ajude no processo de deixar o arquivo nginx.conf mais flexível, ou seja, tanto o host e porta da chamada do php-fpm possam ser definidos como variáveis de ambiente no docker-compose.yaml. 

O resultado final é que quando rodemos docker-compose up -d, tanto o host e a porta do nginx possam ser definidas através de variáveis de ambiente no docker-compose.yaml. 

### Resolução - Docker image

- [lfrichter/laravel_stack](https://hub.docker.com/r/lfrichter/laravel_stack)
- **Lastest is Tag V2**



### Tip

```
docker pull lfrichter/laravel_stack:v2
```

---

## Desafio 2 

Esse desafio é muito empolgante principalmente se você nunca trabalhou com a linguagem Go!
Você terá que publicar uma imagem no docker hub. Quando executarmos:

docker run <seu-user>/codeeducation 

Temos que ter o seguinte resultado: Code.education Rocks!

Se você perceber, essa imagem apenas realiza um print da mensagem como resultado final, logo, vale a pena dar uma conferida no próprio site da Go Lang para aprender como fazer um "olá mundo".

Lembrando que a Go Lang possui imagens oficiais prontas, vale a pena consultar o Docker Hub.

A imagem de nosso projeto Go precisa ter menos de 2MB =)

### Resolução - Imagem Go 

- [lfrichter/codeeducation](https://hub.docker.com/r/lfrichter/codeeducation)



---

<div align="center">

![Docker Image](https://d36jcksde1wxzq.cloudfront.net/be7833db9bddb4494d2a7c3dd659199a.png)

</div>
