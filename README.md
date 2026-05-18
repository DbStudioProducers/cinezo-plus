# CineZo+

Aplicativo de streaming estilo Disney+ com conteudo de cinezo.net, sem login.

## Funcionalidades

- Interface premium estilo Disney+ com tema escuro
- Conteudo carregado do cinezo.net via CORS proxy
- Hero banner rotativo com destaques
- Carrosseis horizontais por categoria
- Busca local em tempo real
- Modal de detalhes com sinopse
- Modo Navegacao integrado (iframe do site original)
- Suporte a Android e iOS via Capacitor
- Sem login, sem cadastro

## Testar no navegador

Abra `www/index.html` em qualquer navegador.

## Build com Codemagic

1. Conecte o repositorio no https://codemagic.io
2. O `codemagic.yaml` ja esta configurado com 3 workflows:
   - **android-debug**: APK de debug (push na branch main)
   - **android-release**: APK assinado (ao criar tag v*)
   - **ios-debug**: Build iOS (push na branch main)
3. Para release Android, configure as variaveis no Codemagic:
   - `KEYSTORE_BASE64`: keystore em base64
   - `KEYSTORE_PASSWORD`: senha do keystore
   - `KEY_ALIAS`: alias da chave
   - `KEY_PASSWORD`: senha da chave

## Estrutura
