# TRb Música — protótipo 0.1

## O que já está incluído
- Modo palco responsivo com letra grande, cifras e avanço manual.
- Importação e visualização do PDF original usando PDF.js.
- Extração de texto por página para inspeção.
- Captura do microfone e medidor de nível de áudio.
- Transcrição experimental em navegadores que oferecem Web Speech API.
- Estrutura PWA instalável quando publicada em HTTPS.

## Limitações importantes
A transcrição do navegador é voltada principalmente à fala. Canto acompanhado por instrumentos pode ser reconhecido incorretamente ou não ser reconhecido. Nesta versão ela apenas tenta sugerir uma linha por correspondência de palavras; não é um alinhador musical confiável. O modo palco manual continua disponível.

A importação do PDF preserva o documento original. A extração de texto não reorganiza automaticamente cifras e letras em PDFs com colunas. A música-piloto está estruturada como exemplo e deve ser revisada com o PDF aberto antes de uso em apresentação.

## Como testar no computador
Abra `index.html` em um navegador moderno. A visualização de PDF depende de conexão para carregar PDF.js. O microfone exige HTTPS ou localhost.

## Como publicar para instalar no Android
1. Crie um repositório GitHub e envie os arquivos desta pasta para a raiz.
2. Em Settings > Pages, publique a branch principal (root).
3. Abra o endereço HTTPS gerado no Chrome do Android.
4. Menu ⋮ > Instalar app / Adicionar à tela inicial.

## Próximo desenvolvimento
1. Revisar a estrutura completa das músicas do PDF.
2. Criar editor de letras e cifras com âncoras por palavra.
3. Implementar alinhamento musical por referência de áudio, testando voz + instrumentos em ensaio.
4. Testar latência, ruído, reverberação e mudanças de andamento em Android real.
