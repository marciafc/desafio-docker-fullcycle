# Desafio Docker FullCycle 3.0

  - Desafio Go
  
  - Desafio Nginx com Node.js
  
## Desafio Go

  - Ao executar ```docker run <seu-user>/fullcycle```, exibir o texto: ```Full Cycle Rocks!!```
  
    - Meu usuário no Docker Hub é marciafcinfo
  
  - Publicar a imagem no docker hub
	
  - A imagem do projeto Go deve ter menos de 2MB

```

$ cd go

$ docker build -t marciafcinfo/fullcycle .

$ docker images

 REPOSITORY               ...   SIZE
 marciafcinfo/fullcycle   ...   1.81MB

$ docker run marciafcinfo/fullcycle

$ docker login

$ docker push marciafcinfo/fullcycle

```


## Referências 

  - Consultas para realizar o desafio Go
    - [Build your Go image](https://docs.docker.com/language/golang/build-images/)
	- [https://github.com/olliefr/docker-gs-ping/blob/main/Dockerfile](https://github.com/olliefr/docker-gs-ping/blob/main/Dockerfile)
	- [Tutorial: Create a Go module](https://go.dev/doc/tutorial/create-module)
	- [GoLang e Docker](https://medium.com/trainingcenter/golang-e-docker-d2d9dedd82c0)
	- [Como fazer um Dockerfile otimizado para Golang](https://www.youtube.com/watch?v=uDCzxwFT2-w)
	- ["Distroless" Container Images](https://github.com/GoogleContainerTools/distroless)
	- [Optimize The Size Of Your Dockerized Go Application Down To 2MB!](https://levelup.gitconnected.com/optimize-the-size-of-your-dockerized-go-application-down-to-2mb-7b826ecb062d)
	- [scratch image](https://hub.docker.com/_/scratch)