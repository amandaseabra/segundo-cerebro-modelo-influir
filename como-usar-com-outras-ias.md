# Como usar o segundo cérebro com outras IAs

O segundo cérebro é feito de arquivos de texto simples. Por isso ele não depende de uma ferramenta: o método funciona no Claude, no ChatGPT e em outras IAs. Este guia mostra o que muda de uma para outra.

**O que é igual em todas:** as pastas, as regras do `AGENTS.md` e o hábito de registrar cada conversa no `LOG.md`.

**O que muda:** a forma de a IA ler os arquivos e a forma de guardar o resultado.

## Quando você usa outra IA, sem o Claude Code

O **Claude Code** é quem grava os arquivos no GitHub por você. Em outras IAs, como o ChatGPT, isso não acontece sozinho, e o caminho é manual:

1. Crie a base a partir do modelo (o GitHub é gratuito).
2. Converse com a IA e peça o texto dos arquivos.
3. Copie cada texto para a sua base no GitHub, como mostrado no passo 3 abaixo.

Dá um pouco mais de trabalho, mas o conhecimento da marca fica igualmente seu, em qualquer ferramenta.

## 1. Dar o contexto à IA

Cada ferramenta aceita arquivos de um jeito, e esses recursos e os limites de cada plano mudam com frequência. Confira na própria ferramenta como enviar arquivos ou pastas. De modo geral, existem três caminhos:

- **Conectar o GitHub**, quando a ferramenta oferece essa conexão.
- **Anexar os arquivos** da base (baixe a pasta do GitHub em Code, Download ZIP).
- **Colar o texto** dos arquivos mais importantes na conversa.

Sempre comece pela pasta `empresa/` e pelas regras do `AGENTS.md`. Se o contexto for grande, envie só a pasta da área do pedido.

**No ChatGPT** (conferido em 01/11 e 03/11/2026): todos os planos permitem anexar arquivos, com limites maiores nos planos pagos. A página de planos lista o recurso **Projetos**, que guarda arquivos de referência para as suas conversas, a partir do plano Plus. O ChatGPT tem um **conector do GitHub que só lê** os arquivos (não grava) e busca o conteúdo quando precisa. Para uma base privada, o app do ChatGPT precisa ter acesso à sua base no GitHub. A central de ajuda da OpenAI indica que o conector começou nos planos pagos (Plus, Pro e Team) e que a oferta mudou em 2026. **Não conseguimos confirmar para os planos Free e Go**: veja na própria ferramenta. Como o ChatGPT só lê, o resultado volta para o GitHub pelo caminho manual do passo 3, abaixo. Os recursos e os limites mudam, então confirme na página de planos antes de assinar.

## 2. Texto para começar uma conversa

Copie e cole, depois anexe ou cole os arquivos:

```text
Você vai trabalhar com o segundo cérebro da minha marca de moda. Leia primeiro
as regras do AGENTS.md e o contexto da pasta empresa. Siga as regras: separe
fato, decisão, hipótese e pendência; não invente dados; não registre senhas,
CPF, cartão nem lista de clientes. Quero trabalhar em: <ASSUNTO>.
Ao final, me entregue o texto pronto de cada arquivo que mudou e uma entrada
para o LOG.md.
```

## 3. Guardar o resultado

Em ferramentas que não gravam direto no GitHub, quem salva é você:

1. Peça à IA o texto final dos arquivos que mudaram e a entrada do LOG.md.
2. No GitHub, abra o arquivo, clique no lápis (Edit), cole o texto e clique em **Commit changes**.
3. Para um arquivo novo, use **Add file, Create new file**.

Para guardar sem perder nada, mude um arquivo por vez e confira o resultado na tela antes de confirmar.

## 4. Levando para outra IA

Quando trocar de ferramenta, a base continua a mesma. Repita o passo 1 e o texto do passo 2. O que a marca já registrou vai junto.

## O que não muda de ferramenta para ferramenta

- A base é privada e não guarda senhas, cartões, CPF nem lista de clientes.
- Informação sem fonte ou data entra como "a confirmar".
- A IA ajuda a escrever e organizar. Quem decide é a liderança da marca.
