# Refúgio Ponta do Seixas

Trabalho final da Unidade I da disciplina Desenvolvimento Front-End para Web (UNIPÊ, prof. Israel Cunha).
É o site de uma pousada fictícia em João Pessoa, na Ponta do Seixas, que segundo a lenda é o primeiro
lugar das Américas a ver o sol nascer. O visitante navega pelas acomodações, pelo lazer, café da manhã
e passeios, e no final pode preencher um formulário pedindo reserva.

Regra principal do trabalho: só HTML, nada de CSS e nada de JavaScript. Então o site é bem simples
visualmente mesmo, sem cores nem fontes personalizadas - o foco aqui foi usar direito as tags e os
atributos que vimos até agora.

## Pré-requisitos

Pra rodar o projeto só precisa de:

- Um navegador (Chrome, Firefox, o que tiver instalado)
- Um editor de código pra ver os arquivos, usamos o VS Code
- Se quiser, a extensão Live Server do VS Code, pra não precisar ficar abrindo o arquivo manualmente toda vez

## Passo a passo

1. Clonar o repositório:

```bash
git clone https://github.com/expnetto/refugio-ponta-do-seixas.git
```

2. Entrar na pasta:

```bash
cd refugio-ponta-do-seixas
```

3. Abrir no VS Code (ou só abrir a pasta pelo próprio editor):

```bash
code .
```

4. Dar duplo clique no `html/index.html` pra abrir no navegador, ou clicar em "Go Live" se estiver
   usando o Live Server.

## Como usar

- O menu fica sempre no topo, em todas as páginas, e no rodapé tem um link pra voltar ao topo.
- Na página **Quartos** dá pra comparar a tabela de tarifas e depois clicar pra ver os detalhes de
  cada acomodação (Suíte Standard, Suíte Vista Mar ou Bangalô).
- Na página do **Bangalô** tem o vídeo do tour, e em **Sobre** tem um áudio com o som do mar.
- Pra reservar, é só ir em **Reservar**, preencher o formulário (os campos com `*` são obrigatórios,
  o próprio navegador não deixa enviar em branco) e ao clicar em enviar cai na página de confirmação.

## Estrutura de pastas

```
refugio-ponta-do-seixas/
├── html/     -> as páginas do site
├── img/      -> fotos e o logo
├── audio/    -> o som do mar
├── video/    -> o vídeo do bangalô
└── README.md
```

Os nomes dos arquivos seguem sempre minúsculo, sem acento e com hífen entre as palavras
(tipo `suite-vista-mar.html`).

## Páginas

| Página | O que tem |
|---|---|
| `index.html` | início, destaques da pousada, avaliações de hóspedes |
| `sobre.html` | história da pousada, áudio do mar, políticas da casa |
| `quartos.html` | tabela de tarifas e resumo de cada acomodação |
| `suite-standard.html` | detalhes da Suíte Standard |
| `suite-vista-mar.html` | detalhes da Suíte Vista Mar |
| `bangalo.html` | detalhes do bangalô, com vídeo do tour |
| `lazer.html` | piscina, redário, programação da semana |
| `cafe-da-manha.html` | cardápio do café da manhã |
| `passeios.html` | passeios oferecidos, valores e dicas |
| `localizacao.html` | mapa e como chegar |
| `reserva.html` | formulário de reserva |
| `obrigado.html` | página que abre depois que o formulário é enviado |

## Limitações

Como não pode ter JavaScript, o formulário de reserva não manda os dados pra nenhum servidor de
verdade - ele só faz a validação padrão do navegador (campo obrigatório, tipo de dado etc.) e depois
abre a página de confirmação. Também não tem como impedir, por exemplo, que a pessoa escolha uma
data de check-out antes do check-in, e o controle de orçamento (aquele "slider") não mostra o valor
que foi arrastado - isso exigiria JS, que é proibido no trabalho.

As fotos, o áudio e o vídeo usados são provisórios, só pra preencher o layout.

## Autores

Eraldo e Davi - turma de Desenvolvimento Front-End para Web, UNIPÊ.
GitHub: [github.com/expnetto](https://github.com/expnetto)
