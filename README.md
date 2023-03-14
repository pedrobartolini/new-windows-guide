# Guia para uma instalação limpa do Windows 10

## Ativar o Windows
Abra o powershell e execute o código abaixo e siga as instruções.
```powershell
irm https://massgrave.dev/get | iex
```

## Ative a aceleração de hardware nativa do windows
Clique com o **botão direito do mouse no desktop**<br>
Clique em **Display settings**<br>
Desça até **Graphical settings**<br>
Ative a opção **Hardware-accelerated GPU Scheduling**<br>
Em **Choose an app to set preference**, escolha *Desktop App*
https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/hardware-accel.png


## Desativar economia de energia
Pesquise por **Power settings**


## Drivers de video
Escolha os drivers correspondentes à sua GPU<br>
[**NVIDIA**](https://www.nvidia.com/download/index.aspx)<br>
[**AMD**](https://www.amd.com/en/support)


## Desinstalar Cortana
Abra o powershell como administrador e execute o código abaixo.
```powershell
Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage
```

## Instale todos os VCREDIST através deste pacote All-In-One
**VCREDIST AIO** https://github.com/abbodi1406/vcredist/releases



