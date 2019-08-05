########################################################
Criador: Lucas Bulegon Mello
E-mail: lucasbmello96@gmail.com
########################################################
Vagrant Provider- Virtual Box

Base Box | VMs de Teste - Ubuntu 14.04 
Base Box | Server VMs - CentOS 7
Endereçamento - 10.0.0.0/24 - Private Network
########################################################

Vagrantfile criado para automatizar a operação de VMs em sistemas que demandem instâncias de banco, webserver e testes.

No arquivo são executados três agrupamentos de máquinas. 

1. VMs de Teste - Com esta configuração podem ser criadas N máquinas, bastando adicioná-las na formatação correta dentro da lista HOSTS.
2. VM de Banco -  Criada no segundo agrupamento de máquinas, sua única diferença é a porta 3306 do convidado exposta como 33306 do hospedeiro.
2. VM Web Server -  Criada no terceiro agrupamento de máquinas, tem a porta 80 do convidado exposta como 8080 do hospedeiro.

Obs. Alterando o bind das portas é possível utilizar as mesmas máquinas virtuais para qualquer propósito, pois não existe configuração de provision com Shell ou derivados que configurar o sistema/aplicação nas máquinas.
