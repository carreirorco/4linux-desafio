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

---

# Relatório

```
Iniciei a terafa por volta das 10h da manhã no dia 24/07/2021.
Testei o acesso ao IP fornecido para realização do desafio e então comecei a configurar o ambiente.
Criei um repositório público no Github e comecei a preparar as configurações do Ansible.
Configurado o inventário do Ansible + teste de conexão, fiz uma análise rápida do servidor disponibilizado.
Nesta análise pude ver alguns detalhes como sistema operacional utilizado, recursos básicos e permissões ao meu usuário.
Por precaução, crei uma maquina virtual na minha máquina e simulei o ambiente para iniciar as alterações.
Então comecei a implementar o Playbook, primeiro criando a role para instalar e configurar o Nginx com os virtual hosts, em seguida utilizei algumas roles públicas para configurar o Docker.
Com o Docker e Nginx em funcionamento, pesquisei sobre as formas de configurar o wordpress em containers como proposto.
Fiz alguns testes utilizando alguns tutoriais e e documentação oficial e então consegui finalizar a primeira instalação do wordpress, em seguida criei a estrutura para replicar essa instalação conforme o solicitado.
Com as instalações do wordpress concluídas e testadas, finalizei a configuração deles via Browser e apliquei os temas diferentes.
Até então todo o ambiente estava funcional, porém ainda no meu ambiente virtualizado, então direcionei para o servidor fornecido e a execução foi concluída sem erros.
Porém ao tentar acessar via Browser notei que da forma que fiz a implementação as portas 8001 até 8003 deveriam estar liberadas para o acesso (acredito que neste ponto acabei não fazendo da forma correta).
Nesse momento configurei o firewall da máquina, mas acredito que a liberação precisa ser feita também na GCP.
Fiz alguns testes para verificar quais eram as portas liberadas no servidor e acredito que o mesmo tenha bloqueado o meu acesso.
Então finalizei esta breve documentação e atualizei o repositório para concluir.
```