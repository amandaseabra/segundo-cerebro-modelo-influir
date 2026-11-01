# Regras desta base

Esta base é o segundo cérebro de uma marca de moda. Guarda o contexto da empresa em arquivos simples. Quem trabalha aqui é o dono da marca ou alguém da liderança, com acesso a todas as áreas. Qualquer IA que leia este arquivo deve seguir estas regras.

## Ao começar

1. Ler o README.md, a pasta `empresa/` e as últimas entradas do LOG.md.
2. Ler também a pasta da área do pedido (financeiro, produto, comercial e assim por diante).
3. Se a pasta `empresa/` ainda estiver vazia, sugerir a skill `comecar` (ou o roteiro de [como-usar-com-outras-ias.md](como-usar-com-outras-ias.md)).
4. Se a base usa Git, conferir se está atualizada antes de editar. Não descartar nada para conseguir atualizar.

## Onde guardar cada coisa

| Assunto | Pasta |
|---|---|
| Quem é a marca, público, metas, decisões da liderança | empresa/ |
| Logo, fontes, cores, brandbook, tom de voz | identidade-de-marca/ |
| Redes sociais, campanhas, calendário, parcerias | marketing-e-comunicacao/ |
| Caixa, resultado, custos, decisões de dinheiro | financeiro/ |
| Coleções, cronograma, preço, estoque, fornecedores | produto/ |
| Vendas, canais, clientes finais, metas | comercial/ |
| Equipe, papéis, rotina, combinados | pessoas/ |
| Como a marca faz as coisas | processos/ |
| O que foi feito em cada conversa | LOG.md |

Criar uma pasta nova só quando houver conteúdo real para ela. Comece com arquivos simples.

## Como escrever

- Português claro e direto, no tom da marca (ver `identidade-de-marca/`).
- Cada informação com **data** e **fonte** (quem disse, qual documento).
- Separar sempre **fato confirmado**, **decisão**, **hipótese** e **pendência**. Nunca transformar uma hipótese em fato.
- Não inventar nomes, números, datas, clientes ou acessos. Se faltar dado, escrever "a confirmar".
- Quando uma informação mudar, atualizar o documento vigente e manter a data da mudança. Não apagar o histórico.
- Exemplos fictícios devem vir marcados como "exemplo".

## Segurança: o que nunca guardar

- Senhas, chaves de acesso, tokens e códigos de verificação.
- Dados de cartão e de conta bancária.
- CPF, endereço e lista de clientes finais.
- Dados pessoais da equipe, como salário e documentos, a menos que a liderança decida guardar e saiba do risco.

A base precisa ser **privada**. Nunca enviar o conteúdo desta base para um repositório público, nem para o modelo de origem. Documentos que a marca quer mostrar ao público ficam em outro lugar.

Arquivos pesados (logo, fontes, fotos, planilhas operacionais) ficam no Drive ou no sistema de origem. Aqui guarda-se o link e a regra de uso.

## Ao encerrar

Toda conversa de trabalho recebe uma entrada no LOG.md, com data, quem trabalhou, apoio de IA, o que foi feito (com links), resultado e pendências. O log não substitui a decisão registrada na pasta da área.

Ao pedir "salvar", seguir a skill `salvar`. O trabalho só conta como salvo quando está na versão principal (main) do GitHub. Não forçar envios, não apagar alterações de outras pessoas e não contornar proteções do repositório.

## Dados atuais

Vendas do dia, caixa de hoje, estoque e agenda ficam nos sistemas da marca. Aqui se registra o link e o papel de cada sistema, e não uma cópia que fica desatualizada.
