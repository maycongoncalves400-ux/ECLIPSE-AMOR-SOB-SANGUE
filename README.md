# ECLIPSE: AMOR SOB SANGUE — Android

Projeto inicial de um RPG 2D narrativo para Android, feito com uma Activity nativa e interface HTML/CSS/JavaScript local dentro de WebView.

## Recursos implementados
- Menu inicial e criação de personagem
- RPG 2D com painel de status: vida, energia, dinheiro, karma e experiência
- Dia/noite e passagem de dias
- Trabalho remunerado
- Missões com escolhas e combate por turnos simplificado
- Relacionamento com Isabella e decisões de afinidade
- Loja, inventário e equipamento
- Mapa de Vesper com locais desbloqueáveis
- Salvamento automático local no aparelho (localStorage)

## Como gerar o APK
1. Instale o Android Studio (versão recente) e o Android SDK 35.
2. Abra a pasta `Eclipse_Amor_Sob_Sangue` no Android Studio.
3. Aguarde a sincronização do Gradle.
4. Selecione **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. O APK de depuração será criado em `app/build/outputs/apk/debug/app-debug.apk`.

Este pacote contém o projeto-fonte. O ambiente de criação não possui Android SDK/Gradle instalado, portanto o APK ainda precisa ser compilado no Android Studio.


## Compilação automática pelo GitHub

O repositório inclui `.github/workflows/build-apk.yml`. Depois de enviar estes arquivos para a branch `main` ou `master`, o GitHub Actions compila o APK automaticamente. Também é possível iniciar manualmente em **Actions → Build ECLIPSE APK → Run workflow**.

Quando a execução terminar, abra a execução concluída e baixe o artefato **ECLIPSE-debug-apk**. Dentro dele estará `app-debug.apk`.

Este é um APK de depuração, adequado para testes e instalação manual. Para distribuição pública na Play Store, será necessário configurar assinatura de release.
