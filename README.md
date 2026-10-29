# ICONOSTAS — Android

Aplicativo Android para abrir o site [ICONOSTAS](https://iconostas-eo.chess777.workers.dev/) dentro do próprio aplicativo, sem encaminhar a navegação HTTPS ao navegador.

## Baixar APK

1. Entre na aba **Actions** do repositório.
2. Abra o fluxo **Gerar APK ICONOSTAS** e clique em **Run workflow** (ou abra a execução automática do push).
3. Aguarde o sinal verde.
4. Na execução concluída, em **Artifacts**, baixe **ICONOSTAS-APK**.
5. Extraia o ZIP e instale **app-debug.apk** no Android.

Este APK é de teste, não é uma versão assinada para distribuição na Play Store. Requer internet. O site é operado por terceiros: confirme a autorização do responsável antes de publicar o aplicativo. Login externo, downloads e outras funções especiais podem exigir ajustes adicionais.

## Tecnologias

Android Java (WebView), Android Gradle Plugin 8.6.1, Gradle 8.7, Java 17, SDK 35, Android 7.0+.

## Personalização

- URL: `MainActivity.java`, constante `HOME`
- Nome: `app/src/main/res/values/strings.xml`
- Ícone provisório: `app/src/main/res/drawable/ic_launcher_vector.xml` e `ic_launcher_foreground.xml`
- Fluxo de compilação: `.github/workflows/build-apk.yml`

O aplicativo não tem anúncios, telemetria própria ou chaves de API.
