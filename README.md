# 4linux-desafio

## Clonar o repositório

```bash
git clone https://github.com/carreirorco/4linux-desafio.git
cd 4linux-desafio
```

## Baixar as roles geerlingguy.docker e geerlingguy.firewall

```bash
ansible-galaxy install geerlingguy.docker -p roles
ansible-galaxy install geerlingguy.firewall -p roles
```

## Fazer apontamento no dns local

Adicionar trecho a seguir no arquivo `/etc/hosts`

```bash
IP_SERVER    4linux.desafio.example
IP_SERVER    app1.4linux.local.com.br
IP_SERVER    app2.4linux.local.com.br
IP_SERVER    app3.4linux.local.com.br
```

## Executar o playbook

```bash
ansible-playbook playbook.yml
```
