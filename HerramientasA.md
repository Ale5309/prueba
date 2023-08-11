
## Herramientas Antimalware para Windows:

1. **Windows Defender:**
   - Descripción: Antivirus incorporado en Windows 10 que ofrece protección en tiempo real.
   - Sitio web: [Windows Defender](https://www.microsoft.com/en-us/windows/comprehensive-security)
   
2. **Malwarebytes:**
   - Descripción: Herramienta antimalware que busca y elimina malware y spyware.
   - Sitio web: [Malwarebytes](https://www.malwarebytes.com/)

3. **Bitdefender Antivirus Free:**
   - Descripción: Una versión gratuita del popular antivirus Bitdefender.
   - Sitio web: [Bitdefender](https://www.bitdefender.com/solutions/free.html)

4. **Avast Free Antivirus:**
   - Descripción: Ofrece protección en tiempo real, escaneos programados y un cortafuegos.
   - Sitio web: [Avast](https://www.avast.com/)

5. **Kaspersky Free Antivirus:**
   - Descripción: Protección básica contra malware y phishing.
   - Sitio web: [Kaspersky](https://www.kaspersky.com/free-antivirus)

6. **ESET NOD32 Antivirus:**
   - Descripción: Antivirus reconocido por su detección efectiva y bajo impacto en el rendimiento.
   - Sitio web: [ESET](https://www.eset.com/)

## Instalación de Windows Defender en Windows 10:

**Paso 1: Acceder a Windows Security:**
1. Haz clic en el ícono del escudo en la barra de tareas o busca "Windows Security" en el menú Inicio.

**Paso 2: Verificar la Protección:**
1. En la ventana de Windows Security, verifica que la protección esté activada.

**Paso 3: Escaneo de Virus y Amenazas:**
1. Haz clic en "Virus & threat protection".
2. Selecciona "Quick Scan" para un escaneo rápido o "Full Scan" para un escaneo completo.
3. Sigue las instrucciones para completar el escaneo.

**Paso 4: Protección en Tiempo Real:**
1. Vuelve a la página principal de Windows Security.
2. Asegúrate de que la protección en tiempo real esté habilitada.

## Instalación de ClamAV en Linux (Ubuntu):

**Paso 1: Instalación:**
1. Actualiza los repositorios y el sistema:
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```

2. Instala ClamAV:
   ```bash
   sudo apt install clamav clamav-daemon -y
   ```

**Paso 2: Actualizar la Base de Datos de Virus:**
```bash
sudo freshclam
```

**Paso 3: Escaneo de Archivos:**
Realiza un escaneo de un directorio:
```bash
sudo clamscan -r /ruta/del/directorio
```

**Paso 4: Eliminar Archivos Infectados:**
Elimina archivos infectados:
```bash
sudo clamscan --infected --remove --recursive /ruta/del/directorio
```

**Paso 5: Ejecutar Demonios:**
Inicia los demonios ClamAV y Freshclam:
```bash
sudo systemctl start clamav-daemon
sudo systemctl start clamav-freshclam
```

