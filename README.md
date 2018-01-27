# angular
Projeto Angular para a Disciplina Linguagem de Script

Foi desensvolvida uma Single Page Aplication (SPA) utilizando o framework Angular, resultado de parceria entre a Google e Microsoft. O projeto foi desenvolvido nos cursos on-line sobre Angular feitos nos sites loiane.training e udemy.com, entre dezembro de 2017 e fevereiro de 2018.

O projeto foi desenvolvido localmente, sendo o Windows 10, Nodejs 8.9.3 e NPM 5.6.0 essenciais para isso. Além do Angular Cli 1.6.5 e o editor de scripts Visual Studio Code, com TypeScript 2.5.3, também foram utilizados o frameworks web Bootstrap 4.0 e Angular 2 Materialize 15.1.10, bem como bibliotecas JavaScript como Jquery 3.3 e Hammer 2.0.8. O Angular tem como requisito recomendável a versão node 6.9.x ou  superior e npm 3.x.x ou superior. Para identificar as respectivas versões instaladas no sistema operacional basta usar os comandos node -v e npm -v, no terminal.

Ao utilizar algumas extensões do VSCode sua produtividade pode aumentar, automatizando a importação de módulos nativos do Angular, por exemplo. A sugestão é de instalar extensões como a de Balram Chavan - chamada de "Angular 2,4 and upcoming latest Typescript Snippets". Outra exensão útil é de John Papa, "Angular v2 TypeScript Snippets". "Auto Import", de steiates, importa automaticamente módulos do Angular, o único problema é que ele mistura os módulos importados do desenvolver com os do Angular. Os módulos do Angular devem ficar no topo, logo abaixo, separados por uma linha, seguem os módulos do desenvolvedor. A extensão HTML snippets facilita o trabalho com HTML, já o "vscode-icons", de Roberto Huertas, identifica cada um dos tipos de arquivos usados nos projetos.

O Nodejs pode ser baixado a partir do site https://nodejs.org.

A instalação de requisitos podem ser feitas via NPM:
TypeScript
npm install -g typescript
Angular CLi:
npm install -g @angular/cli

Materialize
npm install materialize-css --save
npm instalar angular2-materialize --save

O app.module.ts deve deve receber os seguintes códigos, seguindo recomendações do https://angular.io/guide/styleguide

import 'materialize-css';
import { MaterializeModule } from 'angular2-materialize';

Já o arquivo de configuração do angular/cli deve receber na propriedade script:
[
"../node_modules/jquery/dist/jquery.js",
  "../node_modules/hammerjs/hammer.js",
  "../node_modules/materialize-css/dist/js/materialize.js"
  ]

Para criar o projeto, use o comando ng g new nomedoprojeto - que deve começar com uma letra. Em seguida, entre no diretório nomedoprojeto para criar ali componentes, diretivas, serviços, utilizando o Angular cli:

- para criar módulo: ng g m nomedomodulo
- para criar componente: ng g c nomedocomponente
- para criar serviço: ng g s nomedoservico
- para criar diretiva: ng g d nomedadiretiva ????

Os módulos ajudam a organizar uma aplicação por diretórios. O módulo raiz app.module.ts faz referências aos componentes, rotas, serviços bem como dependências de diversos módulos Angular. O módulo possui um template html que mostra os serviços e/ou conteúdo para o usuário final. Já os componentes podem reunir classes, referência ao template ao CSS utilizado e à identificação do componente, que será usada no template.

- O arquivo `README.md` deve ser o guia de seu projeto, e deve possuir: a `descrição do projeto`, os `requisitos mínimos` e `processo de instalação`, `getting started`, `descrição das funcionalidades` e `contato`;
  - Os arquivos e diretórios devem estar bem organizados;
  - E os arquivos devem sempre que possível possuir comentário e boa legibilidade.
* Utilização de temas (90%):
  - *JS Core*:
    * Uso de programação funcional;
    * Validação por meio de RegExp.
  - *JS W3C*:
    * Criação de componentes dinâmicos;
    * Uso de AJAX e JSON.
  - *JS Packages*:
    * Uso de extensões no JS (framework ou bibliotecas), contudo, será exigido a utilização de no mínimo duas extensões inéditas.
    * Webpack e Babel.js
