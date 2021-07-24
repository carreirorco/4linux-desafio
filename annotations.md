# Anotações sobre a realização do desafio proposto

Em primeiro lugar criei um repositório para manter versionado todo o trabalho.

Nesse repositório criei a seguinte estrutura:

```
├── annotations.md (arquivo para manter minhas anotações)
├── chave.pem (chave baixada do email com a proposta do desafio)
├── inventory (inventário com as informações da máquina proposta para realização do desafio)
├── playbook.yml (playbook utilizado para a execução do desafio)
├── README.md (arquivo para documentação final do ambiente)
├── todo.md (arquivo para manter os detalhes do desafio de forma clara para facilitar a execução)
└── .gitignore (arquivo para evitar o versionamento de arquivos sensíveis ou desnecessários)
```

- Para evitar expor a chave privada enviada com o desafio por email configurei o .gitignore
- Para evitar expor o IP do servidor enviado com o desafio por email configuei o meu arquivo local `/etc/hosts` com:

```
IP_ENVIADO_POR_EMAIL    4linux.desafio.example
```

Configurar o wordpress com docker utilizando ansible

https://www.happycoders.eu/devops/ansible-tutorial-setup-docker-mysql-wordpress/

Em determinado momento perdi o acesso ao IP fornecido para realização do desafio então simulei o ambiente utilizando o Vagrant.
