# Roteiro do Desafio

1. Instalar o NGINX na Máquina Local
  - Criar 3 Virtualhosts no NGINX com `proxy_pass` para os domínios abaixo, direcionando as requisições para os contêineres criados no passo 2. 
    - app1.4linux.local.com.br
    - app2.4linux.local.com.br
    - app3.4linux.local.com.br
  - Fique atento na necessidade usar o parâmetro proxy_set_header na sua configuração.

2. Instalar o Docker na Máquina Local
- Criar 3 contêineres com os seguintes nomes:
  -  app1
  -  app2
  -  app3
- Cada container deve ser criado com a implementação de um Wordpress
  - Avalie todas as necessidades para que o Wordpress fique ativo no ambiente.
  - Avalie como o wordpress atenderá pelos domínios do passo 1.
  - Cada container deve ter uma um Tema especifico do Wordpress afim de diferenciar cada aplicação.

  obs: Provisionamentos automatizados não são obrigatórios, mas se forem feitos serão levados em conta.

3. Criar um Relatório Técnico.
- O Relatório Técnico deve contar no mínimo 10 linhas.
- Necessário apresentar um feedback do desafio com as informações de Tempo de Execução, Dificuldades, Implementações Adicionais (se houver), Avaliação do que foi entregue e/ou se faltou algo e, por fim, explicação de como o ambiente ficou provisionado.
- Caso os procedimentos (instalação, configuração, etc) foram versionados associar o Link do repositório na documentação.
- Esse relatório deve ser enviado como resposta desse e-mail, ao finalizar o desafio.
