---
name: salvar
description: Registrar o trabalho da conversa no LOG.md e enviar tudo para a versão principal (main) do GitHub. Usar quando a pessoa pedir para salvar, guardar, compartilhar ou encerrar.
---

# Salvar na base

Objetivo: o trabalho fica registrado no LOG.md e **confirmado na versão principal (main) no GitHub**. A pessoa não precisa saber Git. Explique tudo em linguagem simples.

## Passos

1. **Conferir o ponto de partida.** Veja em qual pasta e branch você está e o que mudou nesta conversa. Confirme que o destino (origin) é a base privada da marca. Nunca envie para outro repositório, e especialmente não para o modelo público.
2. **Revisar o que vai ser salvo.** Leia as mudanças. Garanta que não há senhas, chaves, dados de cartão, CPF nem lista de clientes. Se houver, retire antes de continuar e avise a pessoa.
3. **Registrar no LOG.md** uma entrada com data, quem trabalhou (a pessoa e a IA), o que foi feito com links, resultado e pendências, e a fonte. Não apague entradas anteriores.
4. **Receber o que há de novo.** Rode `git fetch origin`. Se outra pessoa mudou a main, combine com a sua versão usando merge, preservando os dois trabalhos. Em caso de conflito, leia os dois lados e preserve ambos. Se não souber qual vale, pergunte à pessoa.
5. **Gravar e enviar.** Faça o commit das mudanças com uma mensagem clara e envie com `git push origin HEAD:main`.
6. **Conferir.** Confirme que a main do GitHub contém o seu commit (por exemplo, `git fetch origin` e `git merge-base --is-ancestor HEAD origin/main`).

## Nunca

- Forçar o envio (`--force`), usar reset ou apagar alterações para "resolver".
- Esconder trabalho com stash para contornar um problema.
- Mudar o destino do repositório.
- Dizer que salvou antes de conferir a main.

## O que dizer no fim

Se deu certo: "Salvei o seu trabalho. Ele já está na sua base no GitHub e qualquer pessoa autorizada pode abrir a versão atualizada."

Se não deu: "Seus arquivos estão preservados, mas ainda não estão na base do GitHub. Falta <motivo>. O próximo passo é <passo>." Não chame de salvo um trabalho que está só em uma branch temporária.

Se a pessoa pedir "me dê um texto para continuar depois", entregue um parágrafo curto com o objetivo, os arquivos e o que falta.
