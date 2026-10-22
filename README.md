
# PC-PE Agente 2026 - APK com SQLite offline

Esse projeto já está pronto para gerar seu APK.

## O QUE JÁ TEM:
- App com todas as 141 matérias do edital
- Banco SQLite nativo (via @capacitor-community/sqlite) salvando no celular
- Funciona 100% offline no tablet

## COMO GERAR O APK EM 3 MINUTOS:

### Opção 1 - No seu PC (recomendado)
1. Instale Node.js em https://nodejs.org
2. Instale Android Studio
3. No terminal, dentro desta pasta:
   npm install
   npx cap add android
   npx cap copy
   npx cap open android
4. No Android Studio, clique em Build > Build APK(s)

APK vai estar em: android/app/build/outputs/apk/debug/app-debug.apk
Copia pro tablet e instala!

### Opção 2 - Direto online (sem Android Studio)
Use https://appetize.io ou GitHub Actions - projeto já está configurado.

## BANCO SQLITE:
Tabela: checklist_progress
- id (assunto)
- checked (0/1)
- materia
- updated_at

Salvo em: /data/data/br.com.pcpe.checklist/databases/pcpe.db

## PWA ALTERNATIVA (mais rápida):
Se não quiser compilar, use o arquivo www/index.html:
- Abre no Chrome do tablet
- Menu > Adicionar à tela inicial
- Vira um app nativo offline, dados salvos no SQLite do navegador

Bons estudos! - Meta AI
