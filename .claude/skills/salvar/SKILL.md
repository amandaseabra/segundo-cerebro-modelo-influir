---
name: salvar
description: Registrar o trabalho da conversa no LOG.md e enviar tudo para a versão principal (main) do GitHub. Usar quando a pessoa pedir para salvar, guardar, compartilhar ou encerrar.
---

# Salvar na base

Objetivo: o trabalho fica registrado no LOG.md e **confirmado na versão principal (main) no GitHub**. A pessoa não precisa saber Git. Explique tudo em linguagem simples.

## Passos

1. **Conferir o ponto de partida.** Veja em qual pasta e branch você está e o que mudou nesta conversa. Confirme que o destino (origin) é a base privada da marca. Nunca envie para outro repositório, e especialmente não para o modelo público.
2. **Revisar o que vai ser salvo.** Leia as mudanças. Garanta que não há senhas, chaves, dados de cartão, CPF nem lista de clientes. Se houver, retire antes de continuar e avise a pessoa.
3. **Anotar o ponto de volta (backup).** Antes de gravar, veja qual é a versão atual da main (`git rev-parse --short origin/main`). Esse código é o backup: se algo sair errado, a base pode voltar a ele.
4. **Registrar no LOG.md** uma entrada com data, quem trabalhou (a pessoa e a IA), o que foi feito com links, resultado e pendências, e a fonte. Inclua a linha **"Versão anterior (backup)"** com o código do passo 3 e o link `https://github.com/<dono>/<base>/commit/<código>`. Não apague entradas anteriores.
5. **Receber o que há de novo.** Rode `git fetch origin`. Se outra pessoa mudou a main, combine com a sua versão usando merge, preservando os dois trabalhos. Em caso de conflito, leia os dois lados e preserve ambos. Se não souber qual vale, pergunte à pessoa.
6. **Gravar e enviar.** Faça o commit das mudanças com uma mensagem clara e envie com `git push origin HEAD:main`.
7. **Conferir.** Confirme que a main do GitHub contém o seu commit (por exemplo, `git fetch origin` e `git merge-base --is-ancestor HEAD origin/main`).

## Se a pessoa quiser voltar atrás

Siga [como-voltar-atras.md](../../../como-voltar-atras.md). Nunca use reset ou envio forçado para isso: crie uma nova versão com o conteúdo antigo, para o histórico continuar completo.

## Nunca

- Forçar o envio (`--force`), usar reset ou apagar alterações para "resolver".
- Esconder trabalho com stash para contornar um problema.
- Mudar o destino do repositório.
- Dizer que salvou antes de conferir a main.

## O que dizer no fim

Se deu certo: "Salvei o seu trabalho. Ele já está na sua base no GitHub e qualquer pessoa autorizada pode abrir a versão atualizada. Guardei a versão anterior como backup no LOG, caso você precise voltar atrás."

Se não deu: "Seus arquivos estão preservados, mas ainda não estão na base do GitHub. Falta <motivo>. O próximo passo é <passo>." Não chame de salvo um trabalho que está só em uma branch temporária.

Se a pessoa pedir "me dê um texto para continuar depois", entregue um parágrafo curto com o objetivo, os arquivos e o que falta.
