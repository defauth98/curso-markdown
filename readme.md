# Curso de markdown do Roberto Achar

### **O que você vai aprender**:

1. Títulos
2. Parágrafos
3. Negrito e itálico
4. Riscar uma palavra
5. Linhas horizontais
6. Listas não-ordenadas
7. Listas ordenadas
8. Links
9. Imagens
10. Blocos de código

---

### **01 - Títulos**

Para colocar um título usando markdown é preciso usar **#** antes do texto.

Exemplo:

```markdown
# Titulo 1
```

A quantidade de cerquilhas define o tamanha do título **(Podendo ir de 1 a 6)**.

```markdown
# Titulo 1

## Titulo 2

### Titulo 3
```

---

### **02 - Parágrafos**

Um parágrafo no markdown é uma linha comum.

```markdown
Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...
```

O markdown identifica que é preciso pular linha quando inserimos 2 espaços no fim do parágrafo.

```markdown
Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...

Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...
```

---

### **03 - Negrito e itálico**

Para adicionarmos negrito a um texto ou título é preciso colocar \*\* ou -- antes e depois do texto.

Exemplo:

```markdown
Texto em **negrito**

Texto em --negrito--
```

Para o itálico é necessaŕio apenas um \* ou -.

Exemplo:

```markdown
Texto em _itálico_

Texto em -itálico-
```

---

### **04 - Riscar uma palavra**

Para ~~riscar~~ uma palavra no markdowm usando dois ~ antes e depois.

Exemplo:

```markdown
Palavra ~~riscada~~
```

---

### **05 - Linhas horizontais**

Para criar uma linha horizontal e possível usar três caracteres: asterisco( \* ), sinal de subtração ( - ) e o underline( \_ ).

Apartir do terceiro caractere em sequência cria uma linha horizontal. (Também é possível separar os caracteres desde que tenha pelo menos três).

Exemplo:

```markdown
---

---

---

---

---

---

---

---

---
```

---

### **06 - Listas não-ordenadas**

Para criar uma lista não-ordenada é preciso colocar \*, - ou + antes de cada item.

```markdown
- Item 01
- Item 02
- Item 03
```

Podendo também criar subitems dando um tab.

```markdown
- Item 01
  - Subitem 01
  - Subitem 02
  - Subitem 03
- Item 02
- Item 03
```

---

### **07 - Listas ordenadas**

Basta usar uma sequência de números seguidos do ponto final.

Exemplo:

```markdown
1. Item 01
2. Item 02
3. Item 03
```

Mesmo que não seja uma sequência consecutiva, o markdown vai ignorar, por exemplo se for 1, 3 e 5, vai ser colocado 1,2,3.

Exemplo:

```markdown
8. Item 01
9. Item 02
10. Item 03
```

Para criarmos lista ordenada com os numeros que nós escolhemos, tal como um ano de consquista de um título, é necessário criar o item com o ' \ .' no final como se fosse um paragráfo e dar dois espaços para pular linha.

Exemplo:

```markdown
1994\. Brasil  
1998\. França  
2002\. Basil
```

---

### **08 - Links**

Para criar um link é necessário colocar o texto entre colchetes e o link entre parenteses.

Exemplo:

```markdown
[Clique aqui](http://showmethecode.com.br)
```

Usando um texto alternativo:

```markdown
[Show me the code](http://showmethecode.com.br "Show me the code")
```

Usando uma variavel como link:

```markdown
[Clique aqui][site-url]

[site-url]: http://showmethecode.com.br
```

---

### **09 - Imagens**

Para criar uma image é preciso colocar nome entre colchetes e o endereço entre parenteses com sinal de exclamação antes.

Exemplo:

```markdown
![Markdowm](https://avatars3.githubusercontent.com/u/52966246?s=60&u=099dcf52d23e30cbedfb3781de444aa55c2738ca&v=4)
```

Usando uma variavel para guardar o endereço da imagem:

```markdown
![Markdown][image-variable]

[image-variable]: https://avatars3.githubusercontent.com/u/52966246?s=60&u=099dcf52d23e30cbedfb3781de444aa55c2738ca&v=4
```

Adicionando uma imagem com um link:

```markdown
[![Markdowm](https://avatars3.githubusercontent.com/u/52966246?s=60&u=099dcf52d23e30cbedfb3781de444aa55c2738ca&v=4)](http://google.com)
```

Adicionando uma imagem com um link usando variaveis:

```markdown
[![Markdown][image-thumbs]](image-url)

[image-thumbs]: https://avatars3.githubusercontent.com/u/52966246?s=60&u=099dcf52d23e30cbedfb3781de444aa55c2738ca&v=4
[image-url]: http://google.com
```

---

### **10 - Blocos de código**

Para usarmos código em linha basta colocar uma crase antes e depois do código.

Exemplo:

```markdown
Informe os parâmetros `username` e `password` para função `login()`.
```

Se for um codigo javascript com um template string é necessesário usar duas crases

Exemplo:

```markdown
`` const message = `My name is ${name}`; ``
```

Quando se trata de blocos podemos usar 4 indentações.
Exemplo:

```markdown
    // login.js
    const username = 'danielribeiro'
    const password = 'secret123'
    login(username, password)
```

Ou podemos usar 3 crases antes ou depois do codigo. E para adicionar syntax highlighting é preciso colocar o nome da linguagem logo após a primeira sequência de crases.
