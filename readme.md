Temos um cluster que precisamos colocá-lo em produção, a antiga pessoa DevOps que administrava fez uma confusão nesse cluster e agora ele não está mais funcionando.

O Kubernetes está instalado e configurado com CNI e Ingress Controller **corretamente**, precisamos fazer deploy da nossa app o manifesto está em  **/root/desafio-DevOps**, nesse manifesto temos nossas informações **CORRETAS** como portas por exemplo.

A antiga pessoa DevOps tentou criar um **service** e um **ingress** para esse deployment porém não estão funcionando e precisamos ajustá-los e **garantir** que esse service seja acessado **exclusivamente** pelo **ingress**.

Além disso vamos precisar criar um configMap com o nome a sua escolhe, esse configMap deverá conter um chave com o valor do **SEU NOME OU NICK** e deve ser exportada como uma variável de ambiente com o Nome **PLAYER** no nosso deployment localizado em /root/desafio-DevOps

A pessoa DevOps também deixou uma senha criptografada "Z2lyb3BvcHM=" segundo ela nem precisa de chave para descriptografar, crie uma secrets com o nome a sua escolha utilizando essa senha e exporte como uma variável de ambiente com o Nome **CHAVE** no nosso deployment localizado em /root/desafio-DevOps

Regras:
* Não delete nenhum recurso, vamos revisar todos os recursos chave para resolução.
* Pode editar qualquer recurso.
* A CNI está instalada corretamente.
* O Ingress Controller está instalado corretamente.
* O service para acesso  o Ingress Controller está na porta 31211. 
* O Cluster só possui uma máquina.
* Não é permitido fazer o reset do cluster
