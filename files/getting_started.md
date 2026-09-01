#### Movimentar-se em Direção
Movimentar-se em direções diversas.
| Comando | Direção |
| :---: | :---: |
| `h` | Esquerda |
| `j` | Baixo |
| `k` | Cima |
| `l` | Direita |

---
#### Salvar e Sair
Salvar e sair do arquivo.<br> 
Comando `ZZ`

---
#### Deletar
Deletar um caracter.<br>
Comando `x`

Deletar uma linha.<br>
Comando `dd`

Deletar uma quebra de linha.<br>
Comando `J`

---
#### Voltar e Avançar (Undo and Redo)
Desfazer uma ação (voltar).<br>
Comando `u`

Refaz uma ação desfeita (avançar).<br>
Comando `<Ctrl>` + `R`

---
#### Inserir
Inserir um novo texto ANTES da posição do CURSOR.<br>
Comando `i`

Apendar um novo texto APÓS a posição do CURSOR.<br>
Comando `a`

Inserir uma nova linha ABAIXO da posição do CURSOR e ativar o modo de INSERÇÃO.<br>
Comando `o`

---
#### Repetir Comandos
Repetir X vezes uma comando.<br>
Comando `3dd` (Ex.: Deletar 3 linhas = `dd` + `dd` + `dd`)

---
#### Descartar Alterações 
Sair e descartar as alterações realizadas.<br>
Comando `:q!` + `<Enter>`

Recarregar e descartar as alterações realizadas.<br>
Comando `:e!` + `<Enter>`

---
#### Encontrar Ajuda
Exibir a janela de ajuda de pesquisa genérica (documentação completa).<br>
Comando `:help` + `<Enter>`

Exibir a janela de ajuda de pesquisa para algo específico.<br>
Comando `:help i` + `<Enter>` (Ex.: Explicação do comando `i`)

Avançar (clicar) no link contido dentro da janela da ajuda de pesquisa.<br>
Comando `<Ctrl>` + `]`

Retroceder (voltar) no link contido dentro da janela da ajuda de pesquisa.<br>
Comando `<Ctrl>` + `T`

---
#### Movimentar-se entre Palavras
Movimentar-se entre palavras numa mesma linha.
| Comando | Direção |
| :---: | :--- |
| `w` | Primeiro caracter da próxima palavra. |
| `b` | Primeiro caracter da palavra anterior. |
| `e` | Último caracter da próxima palavra. |
| `ge` | Último caracter da palavra anterior. |

---
#### Movimentar-se para o Início/Final da Linha
Movimentar-se entre o início e o final da linha.
| Comando | Direção |
| :---: | :--- |
| `0` | Ir para o início da linha. |
| `$` | Ir para o final da linha. |

---
#### Movimentar-se entre Parenteses, Colchetes e Chaves - (), [] e {}
Movimentar-se entre o inicio e o fim (vice-versa) de parenteses, colchetes e chaves.<br>
Comando `%` (sempre posicionado no item)

---
#### Movimentar-se para uma Linha Específicada
Movimentar-se para a PRIMEIRA linha.<br>
Comando `gg`

Movimentar-se para a ÚLTIMA linha.<br>
Comando `G`

Movimentar-se para uma linha específicada.<br>
Comando `45G` (Ex.: Ir para a linha 45)

---
#### Pesquisar Palavras
Pesquisar palavras simples.
| Comando | Exemplo | Descrição |
| :---: | :--- | :--- |
| `/` | `/casa` + `<Enter>` | Buscar de cima para baixo. |
| `?` | `?casa` + `<Enter>` | Buscar de baixo para cima. |

Navegar entre os resultados da pesquisa.
| Comando | Direção |
| :---: | :--- |
| `n` | Próxima palavra. |
| `N` | Palavra anterior. |

Delimitar pesquisa com inicio e/ou fim de palavras.
| Comando | Exemplo | Descrição |
| :---: | :--- | :--- |
| `\<` | `/\<ca` + `<Enter>` | Palavras que inicializam com CA >> CASA. |
| `\>` | `/ca\>` + `<Enter>` | Palavras que terminam com CA >> MINHOCA. |

---
#### Substituir Textos
Substituir um caracter, palavra ou linha.<br>
Comando `c` + `movimento` (Ex.: `cw` - Da posição do CURSOR até a próxima palavra)

Substituir uma linha.<br>
Comando `cc`

Substituir uma caracter.<br>
Comando `r` + `caracter` (Ex.: `rp` - Caracter da posição do CURSOR para `p`)

---
#### Modo Visual (Seleção)
Selecionar um caracter.<br>
Comando `v`

Selecionar uma linha.<br>
Comando `V`

Selecionar um bloco de caracteres.<br>
Comando `Ctrl` + `v`

Mover-se entre as diagonais do bloco de caracteres.<br>
Comando `o`

---
#### Mover Textos (Cortar e Colar)
Colar um caracter deletado (`x` ou `d`) para a posição posterior ao CURSOR.<br>
Comando `p`

---
#### Copiar Textos (Copiar e Colar)
Copiar um caracter.<br>
Comando `y`

Copiar uma linha.<br>
Comando `yy`

Colar um caracter copiado (`y`) para a posição posterior ao CURSOR.<br>
Comando `p`

---
#### Clipboard (Copiar e Colar)
Copiar utilizando o modo PRIMÁRIO ("Falso" Clipboard).<br>
Comando `"*y`

Colar utilizando o modo PRIMÁRIO ("Falso" Clipboard).<br>
Comando `"*p`

Copiar utilizando o modo CLIPBOARD ("Real" Clipboard).<br>
Comando `"+y`

Colar utilizando o modo CLIPBOARD ("Real" Clipboard).<br>
Comando `"+p`

---
#### Modo de Substituição
Habilitar a subtituição de caracteres, alterando TODA a linha.<br>
Comando `R`

---
#### Edição de Arquivos
Abrir mais de um arquivo em simultâneo (COM registro de abertura + buffer).<br>
Comando `nvim` + `arquivo_1 arquivo_2 ...` (Ex.: `nvim compras.txt boletos.txt`)

Listar os arquivos abertos (COM registro de abertura).<br>
Comando `:args` + `<Enter>`

Redefinir a lista de arquivos abertos (COM registro de abertura).<br>
Comando `:args` + `arquivo_1 arquivo_2 ...` + `<Enter>` (Ex.: `:args mercados.txt boletos.txt`)

Navegar para o próximo arquivo (COM registro de abertura).<br>
Comando `:next` + `<Enter>`

Navegar para o arquivo anteriormente (COM registro de abertura).<br>
Comando `:next` + `<Enter>`

Navegar para o primeiro arquivo (COM registro de abertura).<br>
Comando `:first` + `<Enter>`

Navegar para o último arquivo (COM registro de abertura).<br>
Comando `:last` + `<Enter>`

Abrir um novo arquivo para edição (diretamente na buffer).<br>
Comando `:edit` + `arquivo` + `<Enter>` (Ex.: `:edit compras.txt`)

Salvar um arquivo.<br> 
Comando `:write` + `<Enter>`

Salvar um arquivo (Salvar como...).<br> 
Comando `:saveas` + `arquivo` + `<Enter>` (Ex.: `:saveas verduras.txt`)

Onde parei
https://neovim.io/doc/user/usr_08/#08.1
