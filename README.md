# Multiclauton — app Android de multimídia

Aplicativo Android que reúne quatro recursos de multimídia em telas separadas: câmera, gravador de áudio, player e voz.

Trabalho "App Multimídia" da disciplina **Programação para Dispositivos Móveis III** (ADS, UniSALESIANO Araçatuba), entregue em outubro de 2026.

## Funcionalidades

- **Câmera:** pré-visualização, foto e gravação de vídeo com CameraX
- **Gravador:** grava áudio com `MediaRecorder`, reproduz com `MediaPlayer` e desenha a forma de onda em uma view própria (`WaveformView`)
- **Player:** reprodução de mídia com `MediaPlayer`
- **Fala:** texto para voz (`TextToSpeech`) e reconhecimento de fala (`RecognizerIntent`)

## Stack

- Java
- Android SDK (minSdk 24, targetSdk 36), AppCompat, Material e ConstraintLayout
- CameraX 1.6 (core, camera2, lifecycle, video e view)
- Gradle com Kotlin DSL

## Permissões

Câmera, gravação de áudio, armazenamento e internet. O app pede as permissões em tempo de execução.

## Como rodar

1. Abra a pasta no Android Studio e aguarde a sincronização do Gradle.
2. Execute em um aparelho físico com Android 7 ou mais recente. Câmera e microfone funcionam mal em emulador.

## Estrutura

```
app/src/main/java/com/example/multiclauton/
  MainActivity      menu principal
  CameraActivity    foto e vídeo
  GravaActivity     gravação e reprodução de áudio
  WaveformView      desenho da forma de onda
  PlayerActivity    player
  FalaActivity      texto para voz e reconhecimento de fala
```

## Autor

Fabio Luiz Florêncio da Silva · [github.com/Fabioluiiz22010](https://github.com/Fabioluiiz22010) · [LinkedIn](https://www.linkedin.com/in/fabio-l-florencio/)
