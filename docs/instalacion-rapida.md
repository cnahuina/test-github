# 🚀 Instalación Rápida

Esta guía te ayudará a configurar y ejecutar el proyecto de práctica DevOps
en tu entorno local de manera rápida y sencilla.

## 📋 Prerrequisitos de Software

Antes de comenzar, asegúrate de tener instalado el siguiente software en tu
sistema:

### Requisitos Obligatorios

- **Node.js v18+** - [Descargar desde nodejs.org](https://nodejs.org/)
- **Git** - [Descargar desde git-scm.com](https://git-scm.com/)
- **GitHub CLI (opcional)** - [Descargar desde cli.github.com](https://cli.github.com/)

### Verificación de Prerrequisitos

```bash
# Verificar versión de Node.js
node --version
# Debe mostrar v18.0.0 o superior

# Verificar versión de Git
git --version
# Debe mostrar git version 2.x.x o superior

# Verificar versión de npm
npm --version
# Debe mostrar 8.x.x o superior
```

## 🛠️ Comandos de Instalación

### 1. Clonar el Repositorio

```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/test-github.git

# Navegar al directorio del proyecto
cd test-github
```

### 2. Instalar Dependencias

```bash
# Instalar dependencias del proyecto
npm install

# Verificar que las dependencias se instalaron correctamente
npm list
```

### 3. Configurar el Entorno

```bash
# Crear archivo de configuración local (si es necesario)
cp .env.example .env

# Configurar variables de entorno (editar según sea necesario)
# Nota: Este paso puede variar según la configuración específica del proyecto
```

### 4. Ejecutar el Proyecto

```bash
# Ejecutar en modo desarrollo
npm run dev

# O ejecutar en modo producción
npm start

# Para ejecutar tests
npm test

# Para ejecutar el linter
npm run lint
```

### 5. Verificar la Instalación

```bash
# Verificar que el servidor esté ejecutándose
curl http://localhost:3000

# O abrir en el navegador
# http://localhost:3000
```

## 📸 Resultado Esperado

Después de ejecutar los comandos anteriores, deberías ver una salida similar
a la siguiente:

> **💡 Captura de Pantalla:** Para ver cómo se ve la interfaz completa,
> abre el archivo [`assets/captura-instalacion.html`](assets/captura-instalacion.html)
> en tu navegador.

### En la Terminal

```text
$ npm run dev
> test-github@1.0.0 dev
> node server.js

🚀 Servidor iniciado correctamente
📡 Escuchando en puerto: 3000
🌐 URL local: http://localhost:3000
✅ Entorno: desarrollo
📝 Logs: habilitados
⏰ Tiempo de inicio: 2025-01-13T19:24:30.123Z

[19:24:30] INFO: Aplicación DevOps iniciada
[19:24:30] INFO: Configuración cargada correctamente
[19:24:30] INFO: Base de datos conectada
[19:24:30] INFO: Middleware configurado
[19:24:30] INFO: Rutas registradas
[19:24:30] INFO: ✨ ¡Listo para recibir peticiones!
```

### En el Navegador

Al navegar a `http://localhost:3000`, deberías ver:

```text
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  🎯 Repositorio de Práctica DevOps                          │
│                                                             │
│  ✅ Aplicación ejecutándose correctamente                   │
│  🔧 Entorno: Desarrollo                                     │
│  📊 Estado: Activo                                          │
│  🕐 Uptime: 00:00:15                                        │
│                                                             │
│  📋 Funcionalidades disponibles:                           │
│  • CI/CD Pipeline                                          │
│  • GitHub Actions                                          │
│  • Automatización DevOps                                   │
│  • Documentación técnica                                   │
│                                                             │
│  🔗 Enlaces útiles:                                        │
│  • [Documentación](http://localhost:3000/docs)             │
│  • [API Status](http://localhost:3000/api/status)          │
│  • [Health Check](http://localhost:3000/health)            │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## 🎯 Próximos Pasos

Una vez que tengas el proyecto ejecutándose:

1. **Explora la documentación**: Navega a `http://localhost:3000/docs`
2. **Revisa el CI/CD**: Examina los workflows en `.github/workflows/`
3. **Ejecuta los tests**: Usa `npm test` para verificar que todo funciona
4. **Contribuye**: Crea una rama y envía un pull request

## 🔧 Solución de Problemas

### Error: "node: command not found"

```bash
# Instalar Node.js desde https://nodejs.org/
# O usar un gestor de versiones como nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
nvm install 18
nvm use 18
```

### Error: "npm install" falla

```bash
# Limpiar caché de npm
npm cache clean --force

# Eliminar node_modules y reinstalar
rm -rf node_modules package-lock.json
npm install
```

### Error: Puerto 3000 en uso

```bash
# Encontrar el proceso que usa el puerto
lsof -i :3000

# Cambiar el puerto en la configuración
export PORT=3001
npm run dev
```

## 📞 Soporte

Si encuentras algún problema durante la instalación:

1. Revisa los [Issues del repositorio](https://github.com/tu-usuario/test-github/issues)
2. Consulta la [documentación completa](../README.md)
3. Contacta al equipo de desarrollo

---

**¡Felicidades! 🎉** Has completado la instalación rápida del proyecto DevOps.
Ahora puedes comenzar a explorar y contribuir al proyecto. 