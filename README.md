# Operación Electoral España 2026 - IPOSTEL

Sistema de control, captura y conciliación de datos para el operativo de entrega del voto por correo de las Elecciones de España 2026.

## 📌 Estructura del Proyecto
El sistema se divide en dos componentes principales:
1. **Control Sheet (Google Sheets):** Hojas de cálculo para la captura y consolidación de datos.
2. **Web App (Google Apps Script):** Formulario web para la carga rápida de reportes por parte de Operaciones y CNC.

## 🗂️ Pestañas del Control Sheet
- `CARGA_OPERACIONES`: Recepción internacional en Maiquetía y despacho a centralizadoras (Fase I).
- `CARGA_OPT`: Recepción en oficinas postales, entrega efectiva y novedades (Fase III).
- `CARGA_INTERNACIONAL`: Reporte de avances para la representación en España.
- `DASHBOARD_OBSERVATORIO`: Conciliación automática, métricas de cumplimiento y alertas.

## 🚦 Reglas de Negocio (Orden de Operaciones 009-2026)
- **Prioridad Absoluta:** Piezas recibidas antes de las 2:00 PM salen a primer intento el mismo día.
- **Evidencia Fotográfica:** Ninguna entrega o incidencia es válida sin foto en sitio.
- **Conciliación:** El cierre diario se rechaza si el total despachado (Operaciones) no coincide con el total recibido (CNC/OPT).

## 🛠️ Archivos del Sistema
- `Código.gs`: Lógica del servidor (Apps Script).
- `Index.html`: Menú principal de la Web App.
- `FormularioOperaciones.html`: Interfaz de carga para la Dirección de Operaciones.
- `FormularioCNC.html`: Interfaz de carga para los Jefes de OPT y Gerentes de Estado.

## 🔗 Despliegue
El sistema se ejecuta como una Web App vinculada al Control Sheet. 
*(Nota: Añadir aquí el enlace `/exec` una vez que el problema de pantalla en blanco esté resuelto).*
