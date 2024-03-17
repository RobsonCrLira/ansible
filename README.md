ansible/
├── inventories/
│   ├── production/
│   │   ├── hosts         # Arquivo de inventário para o ambiente de produção
│   │   └── group_vars/   # Variáveis específicas de grupo para o ambiente de produção
│   └── staging/
│       ├── hosts         # Arquivo de inventário para o ambiente de staging
│       └── group_vars/   # Variáveis específicas de grupo para o ambiente de staging
├── roles/
│   ├── common/           # Papel para configurações comuns em todos os hosts
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   └── defaults/
│   ├── webserver/        # Papel para configuração de servidor web
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   └── defaults/
│   └── database/         # Papel para configuração de banco de dados
│       ├── tasks/
│       ├── handlers/
│       ├── templates/
│       └── defaults/
├── playbooks/
│   ├── deploy_webapp.yml   # Playbook para implantar a aplicação web
│   └── provision_servers.yml   # Playbook para provisionar novos servidores
└── ansible.cfg          # Arquivo de configuração global do Ansible
