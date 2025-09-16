FCM - Firebase Cloud Message

O **OneSignal** é uma plataforma de **notificações push** e **mensagens multicanal** usada por desenvolvedores e empresas para se comunicar com usuários em aplicativos móveis, sites e outros canais digitais.

### Principais funcionalidades do OneSignal:

- **Notificações Push Web e Mobile**: Envia notificações para navegadores (Chrome, Firefox) e aplicativos iOS/Android.
- **Mensagens In-App**: Exibe mensagens dentro do aplicativo para engajamento e onboarding.
- **Email e SMS**: Oferece envio de emails e mensagens de texto.
- **Segmentação de Usuários**: Permite enviar mensagens para públicos específicos baseado em comportamento, localização e idioma.
- **Automação e Agendamento**: Suporta campanhas automáticas (como notificações para usuários inativos) e envios programados.

### Manager Workflow

Em projetos Manager Workflow utilizamos o Expo Go que irá gerenciar e cuidar de todas as configurações nativas necessárias para rodar a aplicação no Android e IOS.

### Bare Workflow

No fluxo de trabalho simples você tem controle total. Você pode usar todos os pacotes de Expo SDK, compilações de desenvolvimento e todos os serviços Expo e EAS (Expo Application Service). O Bare Workflow são projetos que não usam o expo prebuild. Ou seja, são projetos em que as alterações são realizadas diretamente nos projetos nativos, em vez de gerá-los automaticamente.

### Como converter um projeto Managed Workflow para Bare Workflow?

Quando você roda o comando expo prebuild pela primeira vez no projeto, e se o projeto é um Managed Workflow, então o projeto será convertido para Bare Workflow criando os diretórios androis e ios.

### Expo Prebuild

O prebuild gera o código nativo antes de compilar. Ele utiliza os plugins de configurações definidas no app.json. O plugin de configuração, por sua vez, gera todas as configurações necessárias no código nativo automaticamente

![[9416b092-3695-453e-8569-c1b76b6f7a71 .png]]
### EAS (Expo Application Service)

Serviços em nuvem para aplicativos Expo e React Native com ferramentas desde a criação, publicação e atualizações de Apps.