# 🔍 CIFRA Forensic Expert — DFIR Skill for Claude

> Convierte a Claude en un **Perito Forense Senior** especializado en 
> análisis forense digital y respuesta a incidentes (DFIR).
> 
> **Autor:** Ing. Arys Alberto Emeterio Ramos  
> **Empresa:** CIFRA — Centro de Investigación Forense y Respuesta a Incidentes  
> **Afiliación:** PEDATEC / PUCMM  
> **Versión:** 1.0.0 | **Estándar:** ISO/IEC 27037

---

## ⚡ ¿Qué hace este skill?

Una vez instalado, Claude asume automáticamente el rol de **Perito Forense Senior de CIFRA** 
cuando detecta cualquier término técnico forense — sin que tengas que pedírselo.

---

## 🛠️ Capacidades incluidas

| Módulo | Herramientas |
|--------|-------------|
| 🖥️ Disco | Autopsy, FTK Imager, TSK, MFTECmd, KAPE |
| 🧠 Memoria RAM | Volatility 3 (pslist, malfind, netscan, yarascan) |
| 📋 Logs | EvtxeCmd, Sysmon, Timeline Explorer |
| 🌐 Red | Wireshark, Zeek, Brim, NetworkMiner |
| 🪟 Artefactos Windows | Prefetch, Shimcache, Amcache, SRUM, LNK |
| 📝 Reportes | ISO/IEC 27037, Fichas CIFRA, Cadena de Custodia |

---

## 📦 Instalación

### Paso 1 — Descargar los archivos
```bash
# Descargar el skill
curl -L -o cifra-forensics.skill \
  https://github.com/solofe01/skill_forense/raw/main/cifra-forensics.skill

# Descargar el hash de verificación
curl -L -o cifra-forensics.skill.sha256 \
  https://github.com/solofe01/skill_forense/raw/main/cifra-forensics.skill.sha256
```

### Paso 2 — Verificar integridad
```bash
# Linux / macOS
sha256sum -c cifra-forensics.skill.sha256

# Windows (PowerShell)
certutil -hashfile cifra-forensics.skill SHA256
# Comparar con: 237db296c86f652b186418cd04ef7924152592da0112773c7603f0d87670b9e7
```

### Paso 3 — Instalar en Claude
```bash
# Crear directorio del skill
mkdir -p /mnt/skills/user/cifra-forensics/

# Extraer contenido
tar -xzf cifra-forensics.skill -C /mnt/skills/user/cifra-forensics/

# Verificar estructura
ls /mnt/skills/user/cifra-forensics/
# Debe mostrar: SKILL.md  references/  assets/  tests/
```Claude debe responder inmediatamente como **Perito Forense CIFRA**.

---

## 📂 Contenido del skill
---

## 🧪 Casos de prueba incluidos

1. Análisis de artefacto Prefetch `.pf`
2. Investigación de volcado de RAM
3. Generación de reporte pericial
4. Documentación de cadena de custodia
5. Análisis de logs EVTX (fuerza bruta)
6. Script Python de automatización forense
7. Consulta procedimental ISO/IEC 27037

---

## 📄 Licencia

Uso libre para investigadores, peritos y profesionales de ciberseguridad.  
Citar al autor y a CIFRA en cualquier uso académico o institucional.

---

*CIFRA — Centro de Investigación Forense y Respuesta a Incidentes*  
*República Dominicana · 2026*

### Paso 4 — Verificar activación
Escribe en Claude cualquiera de estos prompts:
