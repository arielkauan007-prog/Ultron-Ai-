[LEIA-ME.txt](https://github.com/user-attachments/files/33649663/LEIA-ME.txt)
# Ultron IA — projeto para gerar instalador EXE

Este projeto empacota a interface do Ultron IA como aplicativo desktop Windows usando Electron.

## Importante
O arquivo `index.html` é um protótipo. As funções de IA real (respostas inteligentes, pesquisa web e geração de imagens/áudio) ainda precisam ser conectadas a serviços próprios e suas chaves de API. A interface por si só não oferece esses serviços.

## Como gerar o instalador no Windows
1. Instale Node.js LTS em https://nodejs.org/
2. Extraia esta pasta.
3. Abra o terminal nesta pasta e execute:
   `npm install`
   `npm run dist`
4. O instalador será criado na pasta `dist`, com nome semelhante a `Ultron-IA-Setup-1.0.0.exe`.

## Criar o EXE pela nuvem sem instalar ferramentas localmente
A pasta `.github/workflows/build-windows.yml` contém um fluxo de build para Windows. Coloque o conteúdo deste projeto em um repositório GitHub, abra a aba **Actions** e execute **Build Ultron IA for Windows**. Ao terminar, baixe o artefato **Ultron-IA-Installer**, que contém o EXE.

## Nota
O instalador é x64. A primeira execução do build precisa de internet para baixar Electron e suas dependências.
