# 🚀 GUÍA: CÓMO SUBIR A GITHUB

## Paso 1: Crear Repositorio en GitHub

### 1.1 Crear cuenta (si no tienes)
- Ve a: https://github.com/signup
- Crea usuario: `tu-usuario`
- Verifica email

### 1.2 Crear nuevo repositorio
1. Haz clic en `+` → `New repository`
2. **Nombre:** `los-lirios-registro-fv`
3. **Descripción:** "Sistema de registro para instalación FV Hoymiles HMS-1600-4T - Los Lirios"
4. **Público/Privado:** elige según necesidad
5. **Initialize:** Sin README (ya lo tienes)
6. Haz clic en `Create repository`

### 1.3 Copiar URL
```
https://github.com/TU_USUARIO/los-lirios-registro-fv.git
```

---

## Paso 2: Preparar Archivos Locales

### 2.1 Crear carpetas
```bash
mkdir los-lirios-registro-fv
cd los-lirios-registro-fv

# Crear estructura
mkdir registro
mkdir documentacion
mkdir manuales
mkdir plantillas
mkdir scripts
mkdir ejemplos
```

### 2.2 Copiar archivos

```
los-lirios-registro-fv/
├── README.md                          # Ya tienes
├── LICENSE                            # Ya tienes
├── .gitignore                         # Ya tienes
│
├── registro/
│   ├── registro-movil.html            # Tu archivo HTML
│   ├── registro-imprimible.txt        # Tu archivo TXT
│   └── README.md (instrucciones uso)
│
├── documentacion/
│   ├── GUIA_INSTALACION.md
│   ├── ESPECIFICACIONES_TECNICAS.md
│   ├── NORMATIVAS.md
│   └── TROUBLESHOOTING.md
│
└── scripts/
    └── README.md
```

---

## Paso 3: Inicializar Git

### 3.1 Instalar Git
**Windows:**
- Descargar: https://git-scm.com/download/win
- Instalar normalmente

**Mac:**
```bash
brew install git
```

**Linux:**
```bash
sudo apt-get install git
```

### 3.2 Configurar Git
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

### 3.3 Inicializar repositorio local
```bash
cd los-lirios-registro-fv
git init
```

---

## Paso 4: Agregar Archivos

```bash
# Agregar todos los archivos
git add .

# Ver qué se va a subir
git status

# Si quieres excluir algo, editaremos .gitignore
```

---

## Paso 5: Primer Commit

```bash
git commit -m "Inicial: Sistema registro FV Los Lirios v1.0"
```

---

## Paso 6: Conectar con GitHub

```bash
# Agregar remoto (reemplaza URL)
git remote add origin https://github.com/TU_USUARIO/los-lirios-registro-fv.git

# Renombrar rama principal a 'main'
git branch -M main

# Subir al repositorio
git push -u origin main
```

Si pide contraseña:
- **Usuario:** tu-usuario-github
- **Contraseña:** Tu token de acceso personal (no contraseña de GitHub)

### Generar Token Personal

1. GitHub → Settings → Developer settings → Personal access tokens
2. Haz clic en `Generate new token`
3. Nombre: `Los Lirios Registro`
4. Selecciona: `repo` (acceso completo a repositorios)
5. Click en `Generate token`
6. **Copia el token** (no lo verás de nuevo)
7. Úsalo como contraseña en `git push`

---

## Paso 7: Verificar en GitHub

1. Ve a: https://github.com/TU_USUARIO/los-lirios-registro-fv
2. Deberías ver todos tus archivos
3. El README.md se mostrará automáticamente

---

## 📝 Cambios Futuros

### Cuando hagas cambios locales

```bash
# Ver cambios
git status

# Agregar cambios
git add .

# Describir cambio
git commit -m "Descripción del cambio"

# Subir a GitHub
git push
```

### Ejemplo: Actualizar después de instalar más viviendas

```bash
git add ejemplos/registro-actualizado.csv
git commit -m "Agregar registros completados: Bloques 1-3 (18 viviendas)"
git push
```

---

## 🔒 IMPORTANTE: Proteger Datos

### ✅ SÍ subir a GitHub:
- Código (HTML, Python)
- Documentación técnica
- Manuales
- Plantillas vacías
- Configuración

### ❌ NO subir a GitHub:
- Archivos CSV con datos reales
- Información de clientes
- Números de serie reales (en ejemplos públicos)
- Fotos de instalación
- Credenciales

### Cómo proteger:
1. El `.gitignore` ya excluye archivos sensibles
2. Si accidentalmente subes datos:
   ```bash
   git rm --cached archivo.csv
   git commit -m "Remover datos sensibles"
   git push
   ```

---

## 🎯 Estructura Final Recomendada

```
los-lirios-registro-fv/
│
├── 📄 README.md                    ← Documentación principal
├── 📄 LICENSE                      ← Licencia MIT
├── 📄 .gitignore                   ← Archivos a excluir
├── 📄 CONTRIBUTING.md              ← Guía contribuciones
│
├── 📂 registro/
│   ├── registro-movil.html         ← PRINCIPAL - Usar en campo
│   ├── registro-imprimible.txt     ← Para imprimir
│   └── README.md                   ← Instrucciones uso
│
├── 📂 documentacion/
│   ├── GUIA_INSTALACION.md
│   ├── ESPECIFICACIONES_TECNICAS.md
│   ├── NORMATIVAS.md
│   ├── TROUBLESHOOTING.md
│   └── CHECKLIST_SEGURIDAD.md
│
├── 📂 manuales/
│   ├── README.md (enlaces a PDFs)
│   ├── HMS-1600-4T.md (resumen)
│   ├── DTU-Pro-S.md (resumen)
│   └── enlaces-descarga.txt
│
├── 📂 plantillas/
│   ├── formulario-propietario.md
│   ├── plano-instalacion.txt
│   └── checklist-seguridad.txt
│
├── 📂 scripts/
│   ├── README.md
│   ├── validar-serie.py
│   └── exportar-datos.py
│
├── 📂 ejemplos/
│   ├── registro-ejemplo.csv
│   ├── capturas-pantalla/
│   │   ├── registro-01.jpg
│   │   ├── registro-02.jpg
│   │   └── exportacion.jpg
│   └── README.md
│
└── 📂 .github/
    └── ISSUE_TEMPLATE/
        └── reporte-bug.md
```

---

## 🔄 Flujo de Trabajo Recomendado

```
1. Modificas archivos localmente
        ↓
2. git add .
        ↓
3. git commit -m "descripción"
        ↓
4. git push
        ↓
5. ¡Actualización visible en GitHub!
```

---

## 🆘 Problemas Comunes

### "Permission denied"
```bash
# Problema: Token expirado o incorrecto
# Solución: Generar nuevo token personal
```

### "fatal: not a git repository"
```bash
# Solución:
cd los-lirios-registro-fv
git init
git remote add origin https://...
```

### "refusing to merge unrelated histories"
```bash
git pull origin main --allow-unrelated-histories
git push
```

### Necesito revertir un commit
```bash
git log                              # Ver historial
git revert <hash-del-commit>        # Revertir específico
git push
```

---

## 📊 Ver Estadísticas en GitHub

Una vez subido, GitHub mostrará automáticamente:
- 📈 Commits por semana
- 🔄 Actividad del repositorio
- 👥 Contribuyentes
- 📝 Lenguajes usados

---

## 🎓 Recursos GitHub

- [Documentación oficial](https://docs.github.com)
- [GitHub Desktop](https://desktop.github.com) - Interfaz gráfica
- [GitKraken](https://www.gitkraken.com) - Cliente visual

---

## ✅ Checklist Final

- [ ] Repositorio creado en GitHub
- [ ] URL copiada
- [ ] Git instalado y configurado
- [ ] Archivos organizados en carpetas
- [ ] .gitignore presente
- [ ] Primer commit realizado
- [ ] Archivos pusheados a GitHub
- [ ] Verificar en GitHub.com que aparecen los archivos
- [ ] README.md se muestra automáticamente
- [ ] License aparece

---

## 🎉 ¡Listo!

Tu repositorio está en GitHub y listo para:
- ✅ Compartir con tu equipo
- ✅ Colaborar con otros instaladores
- ✅ Mantener histórico de cambios
- ✅ Hacer backup automático
- ✅ Actualizaciones futuras

---

**Próximos pasos:**
1. Sube `registro-movil.html` a repositorio
2. Agrégalo a tu móvil como acceso directo
3. ¡Usa en campo durante las instalaciones!

¿Necesitas ayuda? Consulta: `README.md`
