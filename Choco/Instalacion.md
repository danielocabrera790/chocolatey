## Instalacion de chocolatey
Como paso requerido debemos validar que las políticas de ejecución estén habilitadas, para ello accedemos a PowerShell como administradores y allí ejecutamos lo siguiente:
Get-ExecutionPolicy.
Si el resultado es “Restricted” debemos habilitarlas con el siguiente comando:
Set-ExecutionPolicy AllSigned.
Ingresamos “Sí” para confirmar el proceso, luego ejecutamos de nuevo “Get-ExecutionPolicy” para confirmar el cambio. Procedemos a instalar Chocolatey con el siguiente comando en PowerShell:
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')).
Una vez instalado Chocolatey ejecutaremos el comando “choco” y veremos lo siguiente. Allí veremos la versión de Chocolatey que hemos instalado.
Para usar Chocolatey en Windows 10, vamos a la página principal de Chocolatey y copiamos el comando de instalación y lo pegamos en PowerShell para que dicha aplicación sea instalada en Windows 10.
