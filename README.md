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

### Como executar localmente

> **Pré-requisitos:**  
> Docker instalado em sua máquina

```bash
# 1. Clone este repositório
git clone https://github.com/gabrieldsinfo/python-docker-ci-actions.git
cd python-docker-ci-actions

# 2. Construa a imagem Docker
docker build -t python-demo-app .

# 3. Execute o container
docker run --rm python-demo-app

---
> 📘 Projeto para fins de estudo e demonstração de boas práticas DevOps.
