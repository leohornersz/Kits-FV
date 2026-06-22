# 📂 Estructura Carpetas GitHub - Los Lirios Registro FV

## Copiar/Pegar esta estructura en tu repositorio local

```bash
# PASO 1: Crear estructura completa (bash/terminal)

mkdir -p los-lirios-registro-fv
cd los-lirios-registro-fv

# Crear carpetas principales
mkdir -p registro
mkdir -p documentacion
mkdir -p manuales
mkdir -p plantillas
mkdir -p scripts
mkdir -p ejemplos/capturas-pantalla
mkdir -p .github/ISSUE_TEMPLATE

# Crear archivos iniciales (en Windows, usar 'echo')
echo "# Instrucciones de uso del registro" > registro/README.md
echo "# Documentación técnica" > documentacion/README.md
echo "# Scripts de utilidad" > scripts/README.md
echo "# Ejemplos e imágenes" > ejemplos/README.md
echo "# Manuales técnicos" > manuales/README.md
```

## ESTRUCTURA FINAL ESPERADA

```
los-lirios-registro-fv/                    ← Nombre del repositorio
│
├── 📄 README.md                           ← Documentación principal (YA TIENES)
├── 📄 LICENSE                             ← Licencia MIT (YA TIENES)
├── 📄 .gitignore                          ← Archivos a excluir (YA TIENES)
├── 📄 GITHUB_SETUP.md                     ← Esta guía
│
├── 📂 registro/                           ⭐ CARPETA MÁS IMPORTANTE
│   ├── registro-movil.html                ← USAR EN CAMPO (tu archivo HTML)
│   ├── registro-imprimible.txt            ← Versión para imprimir (tu archivo TXT)
│   ├── registro-ejemplo.csv               ← Ejemplo de datos exportados
│   └── README.md                          ← Instrucciones de uso
│                                             Contenido:
│                                             - Cómo usar en móvil
│                                             - Cómo imprimir
│                                             - Cómo exportar datos
│                                             - Troubleshooting
│
├── 📂 documentacion/                      ⭐ DOCUMENTACIÓN TÉCNICA
│   ├── README.md
│   ├── GUIA_INSTALACION.md                ← 8 pasos instalación
│   ├── ESPECIFICACIONES_TECNICAS.md       ← Datos técnicos detallados
│   ├── NORMATIVAS.md                      ← RD 1699, UNE, CTE, RD 244
│   └── TROUBLESHOOTING.md                 ← Solución de problemas
│
├── 📂 manuales/                           
│   ├── README.md
│   │   Contenido: Enlaces a descargas de PDFs originales:
│   │   - HMS-1600-4T Manual (Hoymiles)
│   │   - DTU-Pro-S Manual (Hoymiles)
│   │   - Smart Meter Manual (Hoymiles)
│   │   - Atersa A-200M Datasheet
│   │   - Solarbloc Especificaciones
│   │
│   ├── HMS-1600-4T-RESUMEN.md            ← Resumen puntos clave
│   ├── DTU-Pro-S-RESUMEN.md               ← Resumen puntos clave
│   └── enlaces-descarga.txt               ← URLs a PDFs originales
│
├── 📂 plantillas/
│   ├── formulario-propietario.md          ← Datos cliente
│   ├── plano-instalacion.txt              ← Template diagrama
│   ├── checklist-seguridad.txt            ← Verificaciones
│   └── checklist-entrega.txt              ← Qué entregar al cliente
│
├── 📂 scripts/                            
│   ├── README.md
│   ├── validar-series.py                  ← Validar SN válidos
│   ├── exportar-a-excel.py                ← CSV a Excel
│   ├── generar-etiquetas.py               ← Crear etiquetas para inversor
│   └── estadisticas.py                    ← Progreso proyecto
│
├── 📂 ejemplos/
│   ├── README.md
│   ├── registro-completo-ejemplo.csv      ← 5-10 registros ejemplo
│   │   Contenido: Datos reales anónimos para referencia
│   │
│   └── capturas-pantalla/
│       ├── registro-movil-01.jpg          ← Captura pantalla registro
│       ├── registro-movil-02.jpg          ← Llenando datos
│       ├── exportacion.jpg                ← Exportando CSV
│       └── README.md                      ← Describir cada captura
│
├── 📂 .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── reporte-bug.md
│   │   └── solicitud-mejora.md
│   │
│   └── workflows/                         ← (Opcional) Automatización
│       └── validar.yml
│
└── 📂 .git/                               ← Creado automáticamente por git init
    └── (Archivos del sistema de versiones)
```

---

## 📋 CONTENIDO DE CADA CARPETA

### 1️⃣ REGISTRO/ (Lo más importante)

**Archivo: registro-movil.html**
```
Tu archivo HTML actual. Contiene:
- Formulario de captura
- Almacenamiento local
- Exportación a CSV
- Estadísticas en vivo
```

**Archivo: registro-imprimible.txt**
```
Tu archivo TXT. Para imprimir:
- Tabla para rellenar a mano
- Verificaciones técnicas
- Notas y observaciones
```

**Archivo: README.md**
```markdown
# Registro de Instalación - Modo de Uso

## 📱 Versión Móvil
1. Abre registro-movil.html en navegador
2. Funciona sin internet
3. Los datos se guardan automáticamente
4. Exporta a CSV cuando termines

## 📄 Versión Imprimible
1. Descarga registro-imprimible.txt
2. Imprime en A4 o A3
3. Lleva al campo
4. Completa a mano
5. Archiva

## 🎯 Campos Obligatorios
- Bloque
- Vivienda
- Inversor HMS

## 📤 Exportación
Haz clic en "Descargar" → Se descarga CSV
```

---

### 2️⃣ DOCUMENTACION/ (Guías técnicas)

**GUIA_INSTALACION.md**
```markdown
# Guía de Instalación Completa

## 8 Pasos

1. Preparación y posicionamiento
2. Cableado CC
3. Cableado CA
4. Conexión a tierra
5. Instalación paneles
6. Indicadores LED
7. Configuración DTU
8. Registro S-Miles Cloud

Cada sección: 
- Procedimiento paso a paso
- Imágenes mentales
- Verificaciones
- Pares de apriete
```

**ESPECIFICACIONES_TECNICAS.md**
```markdown
# Especificaciones Técnicas HMS-1600-4T

## Datos eléctricos
## Rendimiento
## Materiales
## Certificaciones
## Garantía
## Cálculos de producción anual
```

**NORMATIVAS.md**
```markdown
# Normativa Española Aplicable

## RD 1699/2011
Conexión a red baja tensión

## RD 244/2019
Autoconsumo y almacenamiento

## UNE 206006 IN
Protección funcionamiento en isla

## CTE DB-HE
Ahorro de energía

(Resumen de cada norma)
```

**TROUBLESHOOTING.md**
```markdown
# Solución de Problemas

## LED Rojo - No genera energía
Causas: red fuera rango, diferencial disparado, disyuntor...
Solución: verificar voltaje...

## Sin conexión DTU
Causas: WiFi desconectado, fuera rango, interferencias...
Solución: acercar DTU, revisar WiFi...

(Problemas más comunes con soluciones)
```

---

### 3️⃣ MANUALES/

**README.md**
```
# Enlaces a Manuales Oficiales

## Hoymiles (Oficial - Descargar de web)
- HMS-1600-4T: https://www.hoymiles.com/...
- DTU-Pro-S: https://www.hoymiles.com/...
- Smart Meter: https://www.hoymiles.com/...

## Atersa (Oficial - Fabricante paneles)
- A-200M: https://www.atersa.es/...

## Solarbloc (Oficial - Estructura)
- Solarbloc 10°: https://www.solarbloc.es/...
```

---

### 4️⃣ PLANTILLAS/

Archivos .txt / .md para copiar-pegar y personalizar

```
Incluir plantillas:
- Formulario datos cliente
- Plano instalación básico
- Checklist seguridad
- Checklist entrega
```

---

### 5️⃣ SCRIPTS/

Programas Python (opcional) para:
- Validar números de serie
- Convertir CSV a Excel
- Generar etiquetas
- Estadísticas proyecto

---

### 6️⃣ EJEMPLOS/

```
- CSV con registros anónimos de ejemplo
- Capturas de pantalla del registro
- Instrucciones de uso referencia
```

---

## 🚀 CÓMO CREAR ESTA ESTRUCTURA

### Opción A: Manualmente (GUI)
1. Abre tu carpeta GitHub
2. Crea carpetas: registro/, documentacion/, etc.
3. Arrastra archivos .html, .txt, .md
4. Git detecta cambios automáticamente

### Opción B: Terminal (recomendado)

```bash
# Clonar (si ya existe en GitHub)
git clone https://github.com/tu-usuario/los-lirios-registro-fv.git
cd los-lirios-registro-fv

# O crear localmente
mkdir los-lirios-registro-fv
cd los-lirios-registro-fv
git init

# Crear carpetas
mkdir -p registro
mkdir -p documentacion
mkdir -p manuales
mkdir -p plantillas
mkdir -p scripts
mkdir -p ejemplos/capturas-pantalla

# Copiar archivos existentes
cp /ruta/a/registro-movil.html registro/
cp /ruta/a/registro-imprimible.txt registro/
cp /ruta/a/README.md .
cp /ruta/a/LICENSE .
cp /ruta/a/.gitignore .

# Crear README para cada carpeta
touch registro/README.md
touch documentacion/README.md
touch scripts/README.md

# Agregar todo
git add .
git commit -m "Estructura inicial GitHub - Los Lirios v1.0"
git push origin main
```

---

## ✅ CHECKLIST ESTRUCTURA

- [ ] Carpeta `/registro` con archivos HTML y TXT
- [ ] Carpeta `/documentacion` con guías MD
- [ ] Carpeta `/plantillas` con templates
- [ ] Carpeta `/ejemplos` con CSV ejemplo
- [ ] Archivo `README.md` en raíz
- [ ] Archivo `LICENSE` en raíz
- [ ] Archivo `.gitignore` en raíz
- [ ] README.md en cada carpeta principal
- [ ] `.git` creado (si es local)
- [ ] Archivos visibles en GitHub.com

---

## 📝 PRÓXIMOS PASOS

1. **Crear este repositorio en GitHub**
   - Ir a github.com
   - New repository
   - Nombre: `los-lirios-registro-fv`

2. **Descargar este proyecto a tu ordenador**
   ```bash
   git clone https://github.com/TU_USUARIO/los-lirios-registro-fv.git
   ```

3. **Llenar contenido de cada carpeta**
   - Guías técnicas en /documentacion
   - Scripts útiles en /scripts
   - Ejemplos en /ejemplos

4. **Subir cambios**
   ```bash
   git add .
   git commit -m "Contenido completo v1.0"
   git push
   ```

5. **Compartir con equipo**
   ```
   Enlace: https://github.com/TU_USUARIO/los-lirios-registro-fv
   ```

---

**Esta estructura es flexible.** Puedes:
- ✅ Agregar más carpetas si necesitas
- ✅ Crear subcarpetas por bloque
- ✅ Organizar diferente si prefieres
- ✅ Actualizarla conforme avances

Lo importante es que esté **documentado y accesible** para tu equipo.

---

Generated: June 2026 | Version: 1.0
