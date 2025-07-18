# Python + Docker + CI + Actions

Este projeto demonstra a criação de uma aplicação Python containerizada com Docker, com pipeline de integração contínua via GitHub Actions.

A proposta aqui é estruturar um ambiente automatizado que constrói e executa a aplicação em containers a cada alteração enviada ao repositório. Isso permite validar o funcionamento de forma contínua.

### O que está incluído

- Aplicação Python com execução direta
- Dockerfile configurado para empacotar e executar o app
- Workflow no GitHub Actions que:
  - Faz build da imagem
  - Executa o container para validação

---


### Pré-requisitos

Para rodar localmente, você precisa ter instalado:  

- [Docker](https://docs.docker.com/get-docker/)  

> ✅ Não é necessário ter o Python instalado localmente — a imagem Docker já vem com tudo que precisa!

---

### Como executar localmente

1. Clone este repositório:  
    ```bash
    git clone https://github.com/gabrieldsinfo/python-docker-ci-actions.git
    cd python-docker-ci-actions
    ```

2. Construa a imagem Docker:  
    ```bash
    docker build -t nome-da-imagem .
    ```

3. Execute o container:  
    ```bash
    docker run --rm nome-da-imagem
    ```

4. Veja a saída no terminal, que deverá ser:  
    ```
    Aplicação Python rodando em container com sucesso!
    ```

---

### Sobre o workflow GitHub Actions

O pipeline é disparado a cada push na branch `main` e realiza as seguintes etapas:  

- Build da imagem Docker  
- Execução do container para validar a aplicação  

Você pode acompanhar a execução do workflow na aba **Actions** do repositório.

---
> 📘 Projeto para fins de estudo e demonstração de boas práticas DevOps.
