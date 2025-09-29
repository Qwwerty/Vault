#### Github User
```
jorge.luiz@rethink.dev
5edsVSrhsXpLbUd
```

### How to build

Debug -> flutter run --flavor dev -t lib/br_debug.dart -PpropertiesFile=gradle_br
Release -> flutter build apk --release --flavor dev -t lib/br_debug.dart
Release prod → flutter build apk --release --flavor prod -t lib/br_release.dart

### Usuários
[https://docs.google.com/spreadsheets/d/1NAsn3KdMlTTr7Y8kY0Olkv4OuHJdKHZNAoCnkoqUxAE/edit?gid=465579745#gid=465579745](https://docs.google.com/spreadsheets/d/1NAsn3KdMlTTr7Y8kY0Olkv4OuHJdKHZNAoCnkoqUxAE/edit?gid=465579745#gid=465579745)

Usar esse usuário para testar produção
```
ciyiyi9204@daupload.com  
@123Teste
```

### Repository
[https://git.swiftapp.com.br/swift-dev-group/mobile/flutter/global/global-app-flutter/-/tree/socio-swift-merge-global?ref_type=heads](https://git.swiftapp.com.br/swift-dev-group/mobile/flutter/global/global-app-flutter/-/tree/socio-swift-merge-global?ref_type=heads)


------------------------------------------

SOCIO SWIFT: trata-se do programa de fidelidade da empresa Swift. Esse programa visa oferecer benefícios para seus clientes.   
  
accumulationStatus:   
- Acumulo: É um período de 15 dias onde todos os clientes que realizarem uma compra pelo app, site ou pdv. Esse acúmulo depende do valor da compra total.    
  
- Resgate: É um período de 15 dias onde todos os clientes podem usar os valores acumulados. 1) O cashback máximo é de R$60,00; 2) O usuário que não utilizar os seus valores neste período tem seus valores expirados.   
  
ESCOPO DA RETHINK:  
  
-> HOME   
-> EDITAR PERFIL    
-> MENU  
-> EXTRATO   
-> CHECKOUT   
  
* mensagens são diferentes para o cliente que não é sócio. A mensagem padrão vai oferecer o cadastro no programa.   
produto de preço fixo: é aquele que tem um valor fixo para todas as embalagens (ex.: Sal)  
produto de preço variável: é aquele que geralmente está associado ao valor por KG.   
  
  
  
-> swift - cliente   
-> givex - responsável pelo gerenciamento do programa do socio (saldo, histórico)  
-> vtex - plataforma de ecommerce  
  
  
global-app-flutter\apps\features\checkout\lib\presentation\checkout_home\checkout_home_controller.dart

#### Drawio do fluxo da aplicação
https://drive.google.com/file/d/19deAsVeCtHsYV-n15i8WWYy2L2sUk-V8/view