# Amigos Live

Aplicativo em português para conversar e compartilhar a tela com amigos, com contas próprias, salas por convite e até seis pessoas por chamada. Disponível para Windows e Android.

Este repositório distribui os instaladores e o manifesto assinado das atualizações. O código-fonte do aplicativo, o banco de dados e as credenciais do servidor não são publicados aqui.

## Funcionalidades

- Cadastro e login com usuário e senha próprios.
- Salas privadas com entrada por código de convite.
- Chat de texto e chamadas de voz.
- Compartilhamento e visualização de tela.
- Controle de microfone e saída da chamada.
- Verificação de novas versões ao abrir o aplicativo.

## Baixar o aplicativo

Acesse a [versão mais recente](https://github.com/saulomendess06-art/amigos-live-releases/releases/latest) e abra **Assets** para escolher:

| Plataforma | Arquivo |
| --- | --- |
| Windows | `AmigosLive-Setup-<versão>.exe` |
| Android | `AmigosLive-Android-<versão>.apk` |

Baixe apenas o instalador correspondente ao aparelho. O arquivo `amigos-live-update.json` é utilizado pelo atualizador; não precisa ser instalado. Os arquivos automáticos **Source code (zip/tar.gz)** contêm somente os arquivos deste repositório de distribuição, não o código-fonte do aplicativo.

## Instalar e começar

### Windows

1. Baixe o instalador `.exe` da versão mais recente.
2. Feche o Amigos Live, se estiver aberto, e execute o instalador.
3. Crie sua conta ou entre com a conta existente.
4. Crie uma sala ou entre com o código enviado por um amigo.
5. Entre na chamada e permita o microfone quando quiser falar.

O instalador ainda não possui assinatura comercial de código; o Windows pode apresentar um aviso de aplicativo não reconhecido. Confira a origem do download antes de decidir executar.

### Android

1. Baixe o `.apk` da versão mais recente.
2. Abra o arquivo e confirme a instalação no Android. O sistema pode pedir autorização para instalar arquivos do navegador utilizado.
3. Para atualizar, instale por cima da versão existente, sem desinstalar antes.
4. Entre na conta e na sala desejada. Permissões de microfone e captura de tela são solicitadas conforme o uso.

Não existe instalador para iPhone disponível neste repositório.

## Atualizações

O atualizador está incluído a partir do Windows **1.0.4** e Android **1.1.3**. Quem usa uma versão anterior precisa instalar uma dessas versões ou uma posterior manualmente uma última vez.

- **Windows:** verifica ao abrir, baixa em segundo plano e prepara a instalação ao fechar fora de chamada. O botão **Reiniciar para atualizar** é bloqueado durante chamadas.
- **Android:** verifica e prepara o APK ao abrir. O usuário toca em **Instalar atualização** e confirma no instalador do sistema. Na primeira vez, o Android pode pedir autorização para instalar atualizações pelo Amigos Live.
- O aplicativo verifica a assinatura do manifesto e a integridade do arquivo antes de preparar a instalação. Versões iguais ou anteriores não são instaladas pelo atualizador.
- Uma falha ao verificar atualizações não impede continuar usando o aplicativo.

As atualizações dependem da publicação de uma nova versão pelo responsável pelo projeto. Este repositório precisa permanecer público para que os aplicativos façam o download sem exigir autenticação no GitHub.

## Contas e dados

As contas, salas e mensagens ficam no backend do Amigos Live, separado deste repositório. Tornar os instaladores públicos não torna as salas públicas: o acesso às salas continua exigindo conta e convite.

Não publique senhas, tokens, chaves privadas de atualização, chaves de assinatura Android ou cópias do banco de dados neste repositório.

## Limites e disponibilidade

- Até seis participantes por chamada.
- Chamadas e compartilhamento dependem das permissões e da conexão dos aparelhos.
- A retransmissão TURN utiliza um serviço separado. Na configuração de distribuição inicial, o plano sem cartão possui franquia mensal de **500 MB**; ao atingir o limite, a retransmissão pode parar até a renovação, sem cobrança por excedente. Esse limite não corresponde ao download dos instaladores no GitHub.
- Recuperação de senha por e-mail não está implementada na versão inicial.
- Os testes registrados incluem compilação Windows/Android, verificação da assinatura do APK, assinatura/integridade das atualizações e download público dos dois instaladores. A instalação automática final em aparelhos físicos ainda precisa de validação.

## Estrutura deste repositório

```text
README.md       Apresentação e instruções de uso
Releases        Instaladores Windows/Android e manifesto assinado
```

Para compartilhar o aplicativo com seus amigos, envie o [link permanente de downloads](https://github.com/saulomendess06-art/amigos-live-releases/releases/latest).
