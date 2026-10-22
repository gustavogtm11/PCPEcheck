# Deploy na Vercel - PC-PE Checklist

Esse é o pacote CORRETO para subir na Vercel.

## Como fazer deploy (2 minutos):

### Opção 1 - Drag & Drop (mais fácil):
1. Vai em vercel.com/new
2. Na aba "Browse", arrasta ESSA PASTA inteira
3. Deixa assim:
   Framework Preset: Other
   Build Command: (vazio - apaga tudo)
   Output Directory: ./
   Install Command: (vazio)
4. Deploy

### Opção 2 - Via GitHub:
1. Cria repo novo e coloca esses 4 arquivos na raiz
2. Vercel > Import > Seleciona repo
3. Configura:
   Framework Preset: Other
   Root Directory: ./
   Build Command: deixa vazio
4. Deploy

### Por que tava dando erro de "preset"?
Porque na raiz do projeto anterior tinha package.json do Capacitor.
A Vercel tentou detectar como Node e não achou build de Next/Vite.
Com esse pacote limpo (só index.html + manifest + sw + vercel.json) ela entende que é estático.

Depois do deploy, você pode instalar o PWA direto da sua URL da Vercel no tablet!
