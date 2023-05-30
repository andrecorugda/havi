# HAVI ChuGo Dev-Stack
Repository for havi-stellar

# Docker Installation
Install Docker Desktop https://docs.docker.com/desktop/install/windows-install/

# Install WSL-2
Install WSL https://learn.microsoft.com/en-us/windows/wsl/install
Open Powershell Admin
Change WSL Version to 2 Run wsl --set-default-version 2

# Install Ubuntu Distribution
Create username: havi-stellar
Create password: chugo2023
Make sure node js is updated >= v18

# Prepare Chugo Dev Environment
Open Powershell
Go to D: or C: 
mkdir chugo
cd chugo
enter chugo directory and run [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
run Start-BitsTransfer -Source "https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe" -Destination $Env:ProgramFiles\Docker\docker-compose.exe

# Development Stack Installation
npm create refine-app@latest [name of app e.g "havi"]
cd havi or name of the refine app
git clone https://github.com/andrecorugda/havi.git .
docker-compose up -d

