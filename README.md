# python-docker-ci-actions
Este projeto visa demonstrar a criação de uma aplicação Python containerizada com Docker, com pipeline de integração contínua via GitHub Actions.

A proposta aqui é estruturar um ambiente automatizado que constrói e executa a aplicação em containers a cada alteração enviada ao repositório. Isso permite validar o funcionamento de forma contínua.

### O que está incluído

- Aplicação Python com execução direta
- Dockerfile configurado para empacotar e executar o app
- Workflow no GitHub Actions que:
  - Faz build da imagem
  - Executa o container para validação
