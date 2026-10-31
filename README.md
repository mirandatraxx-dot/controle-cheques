# Controle de Cheques — v0.2

Aplicativo Android offline para controle de cheques a pagar.

## O que já existe

- múltiplas empresas no mesmo aplicativo;
- fornecedores separados por empresa;
- cadastro e edição de cheques;
- pesquisa por número, fornecedor ou banco;
- histórico de cheques por fornecedor;
- status A VENCER, VENCIDO, COMPENSADO e CANCELADO;
- atualização automática de cheques vencidos;
- cancelamento de folha/cheque preservando o número e registrando o motivo;
- cancelados fora dos totais a pagar;
- banco local SQLite para funcionamento offline.

## Como gerar o APK sem Android Studio

O projeto já possui um workflow em `.github/workflows/build-apk.yml`.

1. Crie uma conta no GitHub, se ainda não tiver.
2. Crie um repositório novo, por exemplo `controle-cheques`.
3. Envie todos os arquivos deste projeto para o repositório.
4. No GitHub, abra a aba **Actions**.
5. Selecione **Gerar APK - Controle de Cheques**.
6. Clique em **Run workflow** e confirme.
7. Aguarde a compilação terminar com o status verde.
8. Abra a execução concluída.
9. Na seção **Artifacts**, baixe **Controle-de-Cheques-APK**.
10. Extraia o ZIP baixado. Dentro dele estará o arquivo `controle-cheques-debug.apk`.
11. Envie o APK para o celular e instale.

O workflow também compila automaticamente quando houver um `push` na branch `main`.

## Observação importante

Este APK é uma versão de teste/debug. Ele não está assinado para publicação na Google Play. Para instalar diretamente no Android, o APK de debug é suficiente.

O backup automático em nuvem ainda será implementado em uma próxima etapa. Por enquanto, os dados principais ficam no banco local do aparelho.
