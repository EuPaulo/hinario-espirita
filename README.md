# Hinário Espírita
Hinário de músicas espíritas

Construído a partir dos programas LaTeX [songs](http://songs.sourceforge.net/), e [LilyPond](http://www.lilypond.org/).

## Executar
Certifique-se que os programas [songs](http://songs.sourceforge.net/), [LilyPond](http://www.lilypond.org/), [TiMidity++](http://timidity.sourceforge.net/) e [lame](http://lame.sourceforge.net/) estão corretamente instalados. Para a edição de partituras, eu recomendo o [Frescobaldi](http://frescobaldi.org/).
```shell
$ git clone https://github.com/EuAndreh/hinario-espirita.git
$ cd hinario-espirita
$ chmod +x hinario.sh
$ chmod +x boneco.pl
$ ./hinarios.sh

# Para produzir partituras
$ chmod +x partituras.sh
$ ./partituras.sh

# Para produzir arquivos .ogg
$ ./partituras --with-ogg
# ou
$ ./partituras -o
```

## Contribuindo
Se você gostaria de contribuir, inclua a gravação (na qualidade que for - até uma gravação simples de voz e violão realizada no celular) no pull request para que eu possa conferir =].

Se for escrever tanto a partitura quanto a cifra, esforce-se ao máximo para que o tempo das cifras em ambos fique igual.

Lembre-se de escrever as cifras seguindo o padrão já estabelecido.

### LaTeX
Baseie-se no arquivo `template-latex.tex` para inserir uma nova música.

Detalhes:
- Se possível, ajuste o valor `\Huge` para `\LARGE` ou `\Large` na segunda linha do `template-latex.tex` para que a música ocupe apenas 1 página no arquivo `Transparências.pdf`.

### LilyPond
Baseie-se no arquivo `template-lilypond.ly` para inserir uma nova partitura.

Detalhes:
- Seja detalhista quanto às elisões de sílabas e melismas.
- Lembre-se de marcar as voltas e repetições tanto na melodia, quanto na harmonia.

Se for escrever a partitura de uma música que já existe:
```shell
$ ./extrair-letra.pl musicasTex/nome-da-musica.tex
```

Assim, o arquivo LilyPond da música é criado e a letra já é inserida no local apropriado.

## Licença
[![Creative Commons](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

## TODO
- Add favicon
- Tìtulo da música clicável
- Consertar índice com prefixo "A" etc. + acentos
- Mobile responsive website
- Aumentar o tamanhod da donte dos itens do índice
- Consertar tamanho lateral da capa
- Author index?
- tamanho da fonte: número da página e texto do índice

### Partituras faltando
- A Melhor Idade
- Alô, Bom Dia
- Amar como Jesus Amou
- Armadura
- Arte
- Astro Rei

- Bem Viver
- Boa Nova
- Brilhe a Vossa Luz

- Caminhar Servindo
- Cantando a Paz
- Cante e Ame
- Conhecer a Verdade
- Consciência Pura
- Convite ao Vôo

- Dias de Paz

- Ei, Você
- Ele
- Encontro de Luz
- Esta Paz
- Eu e Você
- Eu Posso

- Fraternidade
- Fronteiras

- Hino a Emmanuel
- Hino ao Espiritismo

- Já é Tempo
- Jesus Gosta de Você

- Lírios
- Livro Espírita II

- Mensagem Fraterna

- Novo Dia

- Obrigado, Senhor

- Paz Pela Paz
- Pra Melhorar

- Que Bela Manhã

- Raiz
- Refrão da Alegria

- Segredo
- Seguir com Paulo
- Seguro em Deus
- Ser Gota
- Somos Nós

- Trocando de Roupa

- Um Novo Caminho

- Viver é Tão Bom
