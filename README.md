# Rota Driver — distribuição de atualizações

Este repositório público contém apenas o APK de distribuição assinado e o arquivo `latest.json` usado pelo botão **Verificar atualizações**. O código-fonte permanece no repositório privado.

## Publicar uma versão

1. Gere o APK assinado no workflow privado **APK assinado para distribuição**.
2. Baixe o artefato `rota-driver-release-assinado` e extraia o arquivo `app-release.apk`.
3. Envie **somente** `app-release.apk` para a raiz deste repositório, substituindo o anterior.
4. Atualize `latest.json` com o `versionCode` real do APK e seu endereço HTTPS público.
5. Teste a instalação em um dispositivo antes de anunciar a atualização.

**Nunca publique** o arquivo `.jks`, senhas, tokens, credenciais ou o código-fonte privado.

**Observações:** o Android exige confirmação para instalar APKs. O Google Play Protect pode bloquear aplicativos com permissões sensíveis, e este mecanismo não contorna esse bloqueio. Um APK assinado com chave diferente da versão instalada não pode atualizá-la por cima.
