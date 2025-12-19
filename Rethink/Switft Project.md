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


```

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

```

git config --global user.name "Jorge Luiz Matos Silva"
git config --global user.email jorge.luiz@rethink.dev


```
​@Jonatas Arlindo Pedroso​ no extrato está dando erro

  

curl --location --request GET 'https://global-promotions-apigw-qa.swiftapp.com.br/api/v1/cashback/transaction/history?cpf=64482321095&storeid=41042&pageNumber=1&pageSize=10&sort=DATE_DESC' \  
--header 'regioncode: 1' \  
--header 'user-agent: loja_swift-android-4.1.3-debug' \  
--header 'postal-code: 05118-100' \  
--header 'accept-encoding: gzip' \  
--header 'auth: ' \  
--header 'content-type: application/json' \  
--header 'x-wf-ct-access-token: eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJnaXdheDU4NzkwQGZvZ2RpdmVyLmNvbSIsImlzQ29ycG9yYXRlIjpmYWxzZSwiaXNzIjoic3dpZnQiLCJ2aXAiOmZhbHNlLCJleHAiOjE3NjEyMjkwOTEsInVzZXJJZCI6ImI5NzEzNTMyLWFjZjAtNGFhZS1iNTcxLTE5ODIzNGI2NmNiZCJ9.NIitVYTFAcDuC5HO9KWTpLQkU27s-KI_axXj0ZZ9jy8' \  
--header 'access-token: eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJnaXdheDU4NzkwQGZvZ2RpdmVyLmNvbSIsImlzQ29ycG9yYXRlIjpmYWxzZSwiaXNzIjoic3dpZnQiLCJ2aXAiOmZhbHNlLCJleHAiOjE3NjEyMjkwOTEsInVzZXJJZCI6ImI5NzEzNTMyLWFjZjAtNGFhZS1iNTcxLTE5ODIzNGI2NmNiZCJ9.NIitVYTFAcDuC5HO9KWTpLQkU27s-KI_axXj0ZZ9jy8' \  
--header 'utmsource: android' \  
--header 'token: eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJnaXdheDU4NzkwQGZvZ2RpdmVyLmNvbSIsImlzQ29ycG9yYXRlIjpmYWxzZSwiaXNzIjoic3dpZnQiLCJ2aXAiOmZhbHNlLCJleHAiOjE3NjEyMjkwOTEsInVzZXJJZCI6ImI5NzEzNTMyLWFjZjAtNGFhZS1iNTcxLTE5ODIzNGI2NmNiZCJ9.NIitVYTFAcDuC5HO9KWTpLQkU27s-KI_axXj0ZZ9jy8' \  
--header 'refresh-token: ' \  
--header 'region: br' \  
--header 'content-length: 0' \  
--header 'host: global-promotions-apigw-qa.swiftapp.com.br' \  
--header 'utmcampaign: novoAppGlobal'

"Bad Request: Unknown error loading history"
```