# Visão geral Angular

## O que é o Angular?

Um framework javaScript desenvolvido pelo Google para criação aplicações WEB SPA(single page application) baseada em componentes.

O angular é lançado aproximadamente duas versões por ano.

## Comand Line Interface (CLI)

Interface de linha de comando. E é instalado a partir do camndo abaixo:

- npm i -g @angular/cli

Cria aplicação

- ng new minha-app

## TypeScript

Linguagem criada pela Microsoft - TypeScript - TS.

O código escrito em TypeScript é compilado para JavaScript.

O TypeScript é um superSet do javaScript pois ele tem tudo que o javaScript tem , mas acrescenta  a tipagem forte associado as suas variaveis, interface e outras funcionalidades.

## Arvore de Componentes

Começamos a aplicação através de um componente principal exemplo: myApp que no angular ele chama de app 
component que é o raiz da aplicação, e a prtir desse componente você referencia outros componentes.

<html>
 <img src="/image-readme/arvore.JPG">
</html>


## Conceitos Essenciais

Fluxo de inicialização da aplicação;

- main.ts: ao invés de criar arquivos .js no angular o arquivo é criado como main.ts d typeScript; Esse é o primeiro arquivo para inicializar a aplicação em angular; E o main.ts chama o appModule

- A nossa aplicação em angular é organizada em módulos, uma grande arvore de componentes. E esses módulos
nos dão poderes de criar determinados componentes que estão visíveis apenas dentro do módulo, e isso trás um maior nível de encapsulamento(Encapsulamento vem de encapsular, que em programação orientada a objetos significa separar o programa em partes, o mais isoladas possível.)

- AppModule: por padrão quando você cria uma aplicação em angular já existe um módulo, que é o AppModule, esse é um módulo que será usado para chamar para sua aplicação. Dentro do AppModule haverá um atributo chamado Bootstrap( é inicializar ele vai apontar para o AppComponent);

-AppComponente : AppComponente que é o componente que foi criado por padrão, e apartir do appComponent toda arvore de componentes será chamada;

Processo de Inicialização: -> main.ts será chamado -> o appModule foi carregado e quando appModule foi carregado o primeiro componente que será chamado é o componente que foi declarado no atributo Bootstrap e é exatamente o appComponent, e através do appComponent ele vai fazer referencia para o appHeader, appFooter e outros;


## O que é um Componente?

Componente é um trecho de código que representa um componente visual da sua tela.
Esse componente vai ter um html, um css e ts (seria o arquivo typeScript).
O componete tem comportamento que você vai conseguir através do typeScript, o seu componente tem a estrutura que você consegue através do html e o componente  tem estilo. Ou seja teremos um arquivo.

Quando criamos um componente é gerado uma tag:
 - "<app-home></app-home>" dentro desse componente nós encapsulamos as tres tecnologias

É a partir do arquivo typeScript que nós vamos encontrar tanto o arquivo css, quando o html;
Quando você cria um componente você cria pelo o menos o arquivo typescript. 

## Organização Usando Módulo

- incluir foto

- Anatomia do Módulo

Dentro de um módulo teremos 5 atributos dentro do módulo
 - Declarations ( declara todos os componentes que fazem parte daquele módulo, também diretivas e os pipes), declarations é utilizado principalmente para declarar os componentes que fazem parte do módulo, necessáriamente ele é visivel para fora do módulo, se você quiser deixar um atributo para fora do módulo você tem que deixar dentro de Exports

 - Exports : todos os componentes que vão ser exportados e vão ficar visíveis para fora do módulo, ou seja o exports pode ser tudo que você declaraou em declarations como pode ser uma parte daquilo que você declarou dentro do modulo

  - Imports : é quando temos um módulo que depende de outro modulo, pode ser externo, pode ser uma biblioteca de componentes;

 - Providers: você declara os seus services 
 
 - Bootstrap: onde definimos o componente que será carregado no modulo.O uso do Bootstrap será utilizado apenas em um único módulo, que vai ser aquele modulo de iniciar a aplicação.

## Organização Usando módulo

inserir foto - 