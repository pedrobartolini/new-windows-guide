# Guia para uma instalação limpa do Windows 10

## Ativar o Windows
Abra o powershell e execute o código abaixo e siga as instruções.
```powershell
irm https://massgrave.dev/get | iex
```

## Ative a aceleração de hardware nativa do windows
- Clique com o **botão direito do mouse no desktop**
- Clique em **Display settings**
- Desça até **Graphical settings**
- Ative a opção **Hardware-accelerated GPU Scheduling**
- Em **Choose an app to set preference**, escolha *Desktop App*
<img src="https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/hardware-accel.png" width="800">

## Desativar economia de energia
Pesquise por **Power settings**
Arraste **Performance and Energy** até *Best performance*<br><br>
<img src="https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/power-settings.png" width="800">


## Drivers de video
Escolha os drivers correspondentes à sua GPU

- [**NVIDIA**](https://www.nvidia.com/download/index.aspx)
- [**AMD**](https://www.amd.com/en/support)


## Desinstalar Cortana
Abra o powershell como administrador e execute o código abaixo.
```powershell
Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage
```

## Instale todos os VCREDIST através deste pacote All-In-One
**VCREDIST AIO** https://github.com/abbodi1406/vcredist/releases



