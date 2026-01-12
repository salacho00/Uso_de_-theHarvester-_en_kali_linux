# GUIA HERRAMIENTA THEHARVESTER PARA KALI LINUX
<div align="center">
   <h2>¿Qué es TheHarvester?</h2>
</div>
Es una herramienta de OSINT (Open Source Intelligence) que recopila información pública sobre un objetivo, principalmente:

- Direcciones de correo electrónico
- Subdominios
- Nombres de hosts
- Direcciones IP
- URLs

<div align="center">
   <h2>Instalacion</h2>
</div>
kali linux por defecto tiene preinstalado theHarvester, puedes comprobarlo poniendo en la terminal `sudo theHarvester` y les deberia de aparecer algo asi:

<img width="1008" height="335" alt="Captura de pantalla 2026-01-12 173844" src="https://github.com/user-attachments/assets/6407928a-6031-4bf4-8709-6e2ff07bf1da" />

si por casualidad no tienes el theHarvester en tu kali linux pon este comando: `sudo apt install theharvester` y vuelve a ejecutar el comando `sudo theHarvester`

<div align="center">
   <h2>Funcionamiento</h2>
</div>

la sintaxis basica es `theHarvester -d dominio.com -b fuente`

### Parámetros principales:

- -d: El dominio objetivo que quieres investigar
- -b: La fuente de datos a usar (motor de búsqueda o servicio)
- -l: Limitar resultados (por ejemplo, -l 500)
- -f: Guardar resultados en archivo HTML o XML

### Fuentes de datos disponibles
Algunas de las más útiles:

- google: Google search
- bing: Bing search
- baidu: Motor chino
- dnsdumpster: Subdominios
- hunter: Emails (requiere API key)
- shodan: Dispositivos conectados (requiere API key)
- all: Usa todas las fuentes disponibles

Para saber que fuentes tiene el harvester pon el comando `sudo theHarvester -h`, abra una seccion que diga "SOURCE" ahi podras ver todos las fuentes que tiene tu version de theHarvester

<img width="1107" height="823" alt="Captura de pantalla 2026-01-12 174307" src="https://github.com/user-attachments/assets/cf566bfd-9e39-48ab-b960-c4931e2d189c" />

### Ejemplo de ejecucion
Un ejemplo seria `sudo theHarvester -d tesla.com -b yahoo -l 50`, este comando te devolvera esto:

<img width="568" height="655" alt="Captura de pantalla 2026-01-12 174011" src="https://github.com/user-attachments/assets/d13289bb-29ab-464c-9965-9ca3cde14441" />
<br><br>
Dominios censurados para evitar problemas.
<br><br><br>

TODO ESTO ES CON FINES EDUCATIVOS Y DE ENSEÑANZA PARA MAYOR ACERCAMIENTO CON LAS MAQUINAS Y LA TECNOLOGIA.
