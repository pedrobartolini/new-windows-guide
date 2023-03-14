# Guia para uma instalação limpa do Windows 10

## Ativar o Windows

Abra o powershell e execute o código abaixo e siga as instruções.
```powershell
irm https://massgrave.dev/get | iex
```

## Desinstalar Cortana
Abra o powershell como administrador e execute o código abaixo.
```powershell
Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage
```



