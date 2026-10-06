# Camera Lab — APKs

Repositório de distribuição dos APKs do Camera Lab para Android. O código-fonte do app não está neste repositório.

## Versão atual: 0.2.1

- [Baixar CameraLab-0.2.1-Diagnostico.apk](https://github.com/felipeolimadev/cameralab-apks/releases/download/v0.2.1/CameraLab-0.2.1-Diagnostico.apk)
- [Notas da versão e arquivos](https://github.com/felipeolimadev/cameralab-apks/releases/tag/v0.2.1)
- [SHA-256](https://github.com/felipeolimadev/cameralab-apks/releases/download/v0.2.1/CameraLab-0.2.1-Diagnostico.sha256)

Android 9 ou posterior. APK de aproximadamente 16,8 MiB, variante debug assinada. Pacote: `dev.cameralab`.

## Relatório das câmeras

Na engrenagem da barra superior, toque em **Gerar relatório**. Ao terminar, escolha **Compartilhar** ou **Salvar como…**. O último relatório também pode ser reaberto pelo diagnóstico.

O TXT registra capacidades anunciadas por Camera2 e CameraX: IDs públicos e físicos, características e chaves expostas, formatos, resoluções, foco, exposição, zoom, estabilização, reprocessamento, perfis de faixa dinâmica e cor, além de AUTO, FACE_RETOUCH, BOKEH, HDR e NIGHT. Detalhes de extensões são incluídos conforme o Android e a implementação do fabricante. Falhas de consulta incluem exceções e stack traces, sem serem convertidas em indisponibilidade.

A coleta roda em segundo plano, não dispara fotos e não envia o relatório automaticamente. O inventário não comprova captura funcional nem acesso a recursos privados da câmera stock.

O app mantém o HDR do fabricante via CameraX Extensions, quando disponível para a lente. Não contém fusão RAW própria nem modelos de IA; salva JPEG convencional.

A versão 0.2.1 foi apenas compilada, sem testes no PC ou no aparelho nesta entrega. Geração, compartilhamento e exportação do relatório ainda precisam de validação no telefone.

## Integridade

SHA-256 de `CameraLab-0.2.1-Diagnostico.apk`:

```
fa4c1989b0bf4f0f46825675629444ef5e06f559c3eca1c2932a4f05a4e67e39
```

[Versão anterior 0.2.0 — HDR](https://github.com/felipeolimadev/cameralab-apks/releases/tag/v0.2.0). Novas versões serão publicadas na área de Releases.