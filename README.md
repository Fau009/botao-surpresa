# Botão Surpresa

Uma pegadinha para passar o celular: a página abre direto num botão escrito **“NÃO APERTE”** e ninguém resiste.

**Abrir:** https://fau009.github.io/botao-surpresa/

> Entregue o celular já na página. Quem recebe não vê nenhum menu nem aviso — só o botão proibido.

## Como funciona

1. A tela abre direto no botão vermelho **NÃO APERTE**. Nada revela que é uma brincadeira.
2. No primeiro toque, começa uma **contagem regressiva** que vai esquentando: a tela pisca mais, o som sobe, o botão pulsa e os avisos provocam (“Sério, não aperta” → “VAI, APERTA” → “ÚLTIMA CHANCE”).
3. Se a pessoa apertar o botão — ou se a contagem chegar a zero — vem um **susto** em tela cheia, com som e vibração.
4. Logo depois aparece **“TE PEGUEI!”** com confete e a garantia de que foi só brincadeira, além de um botão para pegar a próxima pessoa.

O susto é sorteado a cada vez, então dificilmente a mesma pessoa vê dois iguais.

## Os 10 sustos

Tela azul (travamento) · Desligando · Atualização do sistema · Baixando vírus · Formatando o disco · Alerta vermelho (sirene) · Câmera invadida · Tela quebrada · Sinal perdido (chuviscos) · Autodestruição.

## É seguro

É **tudo encenação na tela**. A página não mexe no aparelho, não desliga nada, não instala nada e não acessa câmera, arquivos nem qualquer coisa — uma página web não tem como fazer isso. O susto é só visual, com som e vibração, e termina sempre no “Te peguei!”.

## Detalhes técnicos

- O som é gerado na hora (Web Audio) e só começa depois do primeiro toque, porque o navegador exige uma interação antes de tocar áudio.
- A vibração usa `navigator.vibrate` (funciona no Android; o iPhone ignora, sem quebrar nada).
- Um único `index.html` com HTML, CSS e JS puros, sem dependências. Instalável como app (PWA). Publicado pelo GitHub Pages.
