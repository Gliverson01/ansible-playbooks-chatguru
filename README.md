# Configuração_vps

Este projeto foi criado para automatizar o processo de instalação de VPS de forma rápida e padronizada

## Instalação

Para instalar o projeto, siga estas etapas:
1. Clone este repositório.
2. Execute `sudo apt update` para atualizar os pacotes disponíveis;
3. Execute `sudo apt install ansible` para instalar o ansible;
4. Verifique a instalação `ansible --version`;

## Uso

Aqui está como você pode usar o projeto:

Crie um arquivo de hosts Ansible ou edite o arquivo existente para incluir os endereços IP ou nomes de host das suas VPS;
<br/>
No arquivo de hosts deve ser preenchido as seguintes variáveis | VPS-Name `ansible_host=` `ansible_user=` `ansible_ssh_pass=` 
<br/>
Execute o playbook: `ansible-playbook -i seu_arquivo_de_hosts configuracao_vps.yml`;
<br/>
Durante a execução do playbook, você pode ser solicitado a inserir uma *senha*. Digite a senha conforme necessário;

## Estrutura do Playbook

O arquivo configuracao_vps.yml contém as tarefas e configurações que serão aplicadas às suas VPS. Certifique-se de revisar e personalizar este arquivo conforme necessário antes de executar o playbook.
