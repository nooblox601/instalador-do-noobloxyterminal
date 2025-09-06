# instalador-do-noobloxyterminal

Este repositório contém o instalador SFX do NoobloxyTerminal.

## Sobre

Descreva brevemente o propósito do seu projeto aqui.

## Instalação

1. Baixe o instalador SFX mais recente na seção [Releases](https://github.com/nooblox601/instalador-do-noobloxyterminal/releases).
2. Execute o arquivo `.exe` para iniciar a instalação.

## Uso

"@echo off
REM Script para baixar e extrair repositório GitHub como ZIP (Windows)

REM Defina a URL do repositório (altere se necessário)
set REPO_URL=https://github.com/nooblox601/instalador-do-noobloxyterminal/archive/refs/heads/main.zip
set ZIP_NAME=repo.zip

REM Baixar o arquivo ZIP (requer curl ou certifique-se de ter curl instalado)
curl -L %REPO_URL% -o %ZIP_NAME%

REM Extrair o arquivo ZIP (requer PowerShell 5+ ou 7-Zip instalado)
powershell -Command "Expand-Archive -Path '%ZIP_NAME%' -DestinationPath './repo_extraido'"

REM Opcional: Excluir o ZIP após extração
del %ZIP_NAME%

echo Pronto! Os arquivos foram extraídos para a pasta repo_extraido.
pause"

ou.....

# Script PowerShell para baixar e extrair repositório GitHub

# Defina a URL do repositório
$repoUrl = "https://github.com/nooblox601/instalador-do-noobloxyterminal/archive/refs/heads/main.zip"
$zipName = "repo.zip"
$destPath = "repo_extraido"

# Baixar o ZIP
Invoke-WebRequest -Uri $repoUrl -OutFile $zipName

# Extrair o ZIP
Expand-Archive -Path $zipName -DestinationPath $destPath -Force

# Remover o ZIP
Remove-Item $zipName

Write-Host "Pronto! Os arquivos foram extraídos para a pasta $destPath."
Pause

## Contribuição

Pull requests são bem-vindos. Para mudanças maiores, por favor abra uma issue primeiro para discutir o que você gostaria de modificar.

Certifique-se de atualizar os testes conforme necessário.

## Licença

[MIT](LICENSE)
# obrigado or ler ate aqui lol
