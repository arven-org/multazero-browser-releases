# MultaZero Browser Studio

Aplicativo desktop para gravar e repetir consultas em portais, com extração de dados para revisão e API local. Este repositório só publica os instaladores e as atualizações; o código-fonte é privado.

## Baixar

Abra a [versão mais recente](https://github.com/arven-org/multazero-browser-releases/releases/latest) e baixe o arquivo do seu computador:

| Computador | Arquivo |
|---|---|
| Windows 10 ou 11 (64 bits) | `MultaZero-Browser-Studio-Setup-X.Y.Z.exe` |
| Mac com Apple Silicon (M1 ou mais novo) | `MultaZero-Browser-Studio-X.Y.Z-arm64.dmg` |
| Mac com processador Intel | `MultaZero-Browser-Studio-X.Y.Z-x64.dmg` |

Requisito: Google Chrome instalado (usado nas execuções em segundo plano).

## Instalar no Windows

Dê dois cliques no instalador. Ele instala só para o seu usuário, sem pedir administrador, cria atalhos na Área de Trabalho e no Menu Iniciar e abre o app.

O instalador ainda não tem assinatura digital. Se aparecer "O Windows protegeu o computador", clique em **Mais informações** e depois em **Executar assim mesmo**.

## Instalar no Mac

Abra o `.dmg` e arraste o MultaZero Browser Studio para **Aplicativos**.

O app ainda não é assinado pela Apple, então na primeira abertura o macOS avisa que não pôde verificá-lo. Feche o aviso, abra **Ajustes do Sistema → Privacidade e Segurança**, role até o fim e clique em **Abrir Mesmo Assim** ao lado do nome do app. É preciso fazer isso uma vez a cada versão nova.

## Atualizações

- **Windows:** o app procura versões novas ao abrir e a cada 4 horas, baixa em segundo plano e mostra **Reiniciar e atualizar** na barra de cima. Se você preferir, a atualização instala sozinha quando o app for fechado. Ele nunca reinicia no meio de uma gravação ou execução.
- **Mac:** o app mostra **Baixar vX.Y.Z** na barra de cima quando sai uma versão nova. Baixe o `.dmg` e arraste o app para Aplicativos, substituindo o antigo.

Fluxos, histórico, PDFs e acessos salvos continuam depois de atualizar.

## Desinstalar

- **Windows:** Configurações → Aplicativos → MultaZero Browser Studio → Desinstalar. Remove o programa, os atalhos, os registros do instalador e o cache de atualizações. Seus fluxos, histórico, PDFs e acessos salvos ficam em `%APPDATA%\MultaZero Browser`, para não se perderem numa reinstalação; apague essa pasta se quiser remover tudo.
- **Mac:** arraste o app de Aplicativos para o Lixo. Os dados ficam em `~/Library/Application Support/MultaZero Browser`.

## Conferir o download

Cada versão traz `SHA256SUMS.txt` com a soma de cada instalador. Para comparar:

- Windows (PowerShell): `Get-FileHash .\MultaZero-Browser-Studio-Setup-X.Y.Z.exe`
- Mac (Terminal): `shasum -a 256 MultaZero-Browser-Studio-X.Y.Z-arm64.dmg`
