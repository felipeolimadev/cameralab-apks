# Camera Lab — APKs

Repositório de distribuição dos APKs do Camera Lab para Android.

## Versão atual: 0.3.0

- [Baixar CameraLab-0.3.0-Modos-HDR.apk](https://github.com/felipeolimadev/cameralab-apks/releases/download/v0.3.0/CameraLab-0.3.0-Modos-HDR.apk)
- [Notas da versão e arquivos](https://github.com/felipeolimadev/cameralab-apks/releases/tag/v0.3.0)
- [SHA-256](https://github.com/felipeolimadev/cameralab-apks/releases/download/v0.3.0/CameraLab-0.3.0-Modos-HDR.sha256)

Android 9 ou posterior. APK de aproximadamente 16,8 MiB, variante debug assinada. Pacote: `dev.cameralab`, versionCode 4.

## Seleção de processamento

Toque no botão HDR da barra superior para alternar entre os modos disponíveis para a câmera selecionada. Segure o botão para abrir a lista completa com descrições e disponibilidade.

A sequência é Foto normal → HDR de cena → Ultra HDR → HDR do fabricante → Auto do fabricante → Noturno do fabricante. Modos indisponíveis ou que falharam são pulados. Auto e Noturno têm rótulos próprios; Auto não garante aplicação de HDR.

- HDR de cena é experimental: solicita os controles públicos Camera2 quando anunciados e registra os valores retornados. A aceitação dos controles não comprova melhora de qualidade.
- Ultra HDR exige Android 14 ou posterior e suporte anunciado pelo CameraX. O app solicita JPEG_R, verifica a presença de gain map na foto salva e preserva o arquivo original. A exibição HDR depende de visualizador e tela compatíveis.
- HDR, Auto e Noturno do fabricante usam as respectivas CameraX Extensions, conforme a disponibilidade por câmera.

Os modos são exclusivos. O flash fica desligado nos modos de processamento e o controle EV fica indisponível no HDR de cena. Em falha, o app tenta voltar à Foto normal e desabilita o modo afetado naquela câmera até a próxima abertura. Fotos já salvas são preservadas; capturas que falharam precisam ser disparadas novamente.

Esta versão ainda não contém o HDR próprio com fusão de múltiplos quadros nem modelos de IA.

## Relatório das câmeras

Na engrenagem da barra superior, toque em **Gerar relatório**. Ao terminar, escolha **Compartilhar** ou **Salvar como…**. O último relatório também pode ser reaberto pelo diagnóstico.

O TXT registra capacidades anunciadas por Camera2 e CameraX, formatos de saída, extensões, modo solicitado/vinculado e até oito evidências recentes de captura ou falha. A coleta não dispara fotos nem envia o relatório automaticamente. O inventário não comprova captura funcional nem acesso a recursos privados da câmera stock.

## Validação e integridade

A versão 0.3.0 foi compilada com sucesso. Não foram executados testes no PC ou no telefone nem instalados programas nesta entrega. Qualidade, estabilidade e transições precisam de validação em aparelho.

SHA-256 de `CameraLab-0.3.0-Modos-HDR.apk`:

```
e03cd7c1d4ad55c1794976642baca9f13883c3b7dcf5de9855f17efe2c764f64
```

O repositório publica APKs e documentação de distribuição; código-fonte, fotos e relatórios pessoais não são enviados.

[Versão anterior 0.2.1 — diagnóstico](https://github.com/felipeolimadev/cameralab-apks/releases/tag/v0.2.1).
