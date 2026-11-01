# Como voltar atrás

Enviou algo errado? Sem pânico. O GitHub guarda **todas as versões** da sua base, e cada salvamento anota no [LOG.md](LOG.md) qual era a versão anterior (o backup). Você nunca perde o que já foi salvo.

## Jeito mais simples: peça à IA

Copie e cole na conversa:

```text
Quero voltar atrás. Olhe o LOG.md, veja o salvamento de <DATA> e restaure
<ARQUIVO ou "tudo"> para a versão anterior (backup). Não apague o histórico:
crie uma nova versão com o conteúdo antigo e registre no LOG.
```

A IA cria uma **nova versão** com o conteúdo antigo. O que estava errado continua no histórico, mas deixa de valer.

## Jeito manual, pelo GitHub

1. Abra o arquivo no GitHub e clique em **History** (Histórico).
2. Encontre a versão certa pela data e clique nos três pontinhos, depois em **View file** (Ver arquivo).
3. Copie o texto, volte ao arquivo atual, clique no lápis (Edit), cole e clique em **Commit changes**.

## O que nunca fazer

- Pedir à IA para **apagar o histórico**, usar *reset* ou *force push*. Isso destrói os backups.
- Voltar atrás sem registrar no LOG. Anote sempre o que foi restaurado e por quê.

## Se o erro foi enviar algo sensível

Senha, dado de cartão, CPF ou lista de clientes que foram salvos **continuam no histórico**, mesmo depois de apagados do arquivo. Nesse caso:

1. Troque a senha ou o acesso imediatamente.
2. Avise a Influir ou peça ajuda de alguém de tecnologia: limpar o histórico exige um procedimento específico.
3. Confirme que o repositório está como **Private**.
