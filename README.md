# THUNDERAPP

* Este projeto é um template para usar usar nos aplicativos do flutter
Muitas coisas já foram configuradas. O Template vem com uma implementação básica do provider. 
O template vem com diversos comentários de documentação. Siga-os. 

## Pacotes usados
  ### Provider 
   -  Provider é um gerenciador de estados para o flutter. É um pacote simples de gerenciamento, mas também poderosíssimo. Sua implementação é feita baseada em árvores. No caso, a implementação deve ser feita no topo da árvore e seus decendentes podem acessar de qualquer lugar do app. Alguns exemplos estão implementados no app. Documentação: https://pub.dev/packages/provider
   ### Firebase
    - Firebase é um conjunto de ferramentas para gerenciamento de pequenos serviços de back end, como Storage, Notifications, Database etc. Este pacote é recomendadíssimo pois sua instalação é fácil e seu uso é extenso.
   ### Intl
    - INTL é usado para internacionalização, conversão de horários, moedas etc. O melhor pacote quando se trata de converter e usar valores monetários etc.
   ### Url_launcher
    - Necessário para apontar links na web externamente.
   ### Path Provider
    - Path provider dá acesso às apis de caminho do os. File system, folders etc. 
   ### File picker
    - API usada para selecionar arquivos que estão nos caminhos do OS
   ### Image picker
    - API Usada para selecionar arquivos, porém com o refinamento de imagens
   ### Dio
    - Cliente HTTP usado para fazer requisições HTTP. Dio é o melhor cliente http para flutter, extremamente fácil de usar
   ### Logging
    - API de logger, bom para capturar logs no flutter.
# Arquitetura, organização de pastas ETC.
  ## O projeto já vem com um padrão de pastas pré definido. É aconselhável que se siga esse padrão para melhor manutenção de código e para padronização do projeto.
    ### Assets:
      - Esta pasta guarda todos os arquivos de assets do projeto. Coloque aqui todos os arquivos 
      externos do projeto como: imagens, ícones, jsons pré carregados etc...
    ##Uso do Gerenciador de estado e estrutura de arquivos e pastas
      - Todas as telas devem seguir esse padrão: 
          -- NAME_OF_THE_SCREEN_FOLDER
              -- name_of_the_screen_screen.dart
              -- **_controller.dart
              -- **_repository.dart
         Onde o nome da tela deve ser o prefixo para o controller e o repositório.
    ##Componentes
      - Os componentes são de dois tipos: os locais e os globais. Os locais são componentes que pertencem a determinada tela ou outro componente, estes não são compartilhados por todo o projeto, servido apenas para um propósito local. Já os componentes globais são aqueles que são compartilhados por todo o app, podendo ser reutilizado em qualquer tela ou outro componente. Esses componentes devem ficar numa pasta chamada "shared". 
    
## Como começar
Baixe o template, renomeie suas dependências de caminho
Dê um flutter pub get para pegar as dependências.
Diversos comentários de todo estão feitos no app, você deve mudar o nome do app nos seguintes arquivos:
- Pubspec.yaml
- AndroidManifest nível app
- AndroidManifest nível projeto
- Build.gradle nível app
### Divirta-se
