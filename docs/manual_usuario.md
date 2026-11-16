# Manual de Usuario — Mosquito Data Management System Galápagos

## Inicio de sesión

Al abrir la aplicación se mostrará la ventana de inicio de sesión.

| Rol | Permisos |
|-----|----------|
| **admin** | Acceso completo: datos, gráficos, mapa, usuarios |
| **analista** | Carga y análisis de datos, exportación |
| **visor** | Solo visualización (sin guardar ni exportar) |

---

## Cargar datos

1. Ve a la pestaña **Datos**.
2. Haz clic en **Cargar Excel** y selecciona tu archivo `.xlsx` o `.xls`.
3. La aplicación detecta automáticamente las columnas. Si alguna no se reconoce,
   aparecerá el diálogo de mapeo de columnas para asignarlas manualmente.
4. Una vez cargado, los datos quedan disponibles en todas las pestañas.

### Formato del archivo Excel

El archivo debe contener al menos estas columnas (los nombres exactos pueden variar;
la app los detecta automáticamente):

| Columna | Descripción |
|---------|-------------|
| Codigo de ovitrampa | Identificador único de cada trampa |
| Semana epidemiologica | Número de semana (1–52) |
| Fecha de instalacion | Fecha en que se instaló la trampa |
| Fecha de inspeccion | Fecha de recolección/inspección |
| Ovitrampa instalada | 1 = instalada, 0 = no instalada |
| Ovitrampa recuperada | 1 = recuperada, 0 = no recuperada |
| Huevos enteros Ae. aegypti | Conteo de huevos viables |
| Huevos no viables Ae. aegypti | Conteo de huevos no viables |
| Huevos rotos Ae. aegypti | Conteo de huevos rotos |
| Total de huevos Ae. aegypti | Suma total de huevos |
| Coordenada Y | Latitud (decimal) |
| Coordenada X | Longitud (decimal) |

---

## Historial de datos

El historial está disponible en la barra superior (**Historial**).

Los datasets de Galápagos 2025–2026 vienen precargados:
1. Clic en **Historial**.
2. Selecciona el dataset deseado.
3. Clic en **Cargar seleccionado** (o doble clic en la fila).

---

## Pestaña Gráficos

Muestra análisis temporal de los datos cargados:
- Evolución de huevos por semana epidemiológica.
- Comparación por sector/localidad.
- Correlación entre variables.

**Filtrar por localidad:** Si los datos tienen más de una localidad (p. ej., Bellavista / Miramar),
aparecerá el selector `Localidad:` en la barra superior de esta pestaña.

---

## Pestaña Mapa

Visualización geográfica de las ovitrampas:
- **Clusters:** agrupa ovitrampas cercanas para mejor visualización.
- **Mapa de calor:** muestra densidad de huevos por zona.
- Haz clic en cada marcador para ver los detalles de la trampa.

**Filtrar por localidad:** Igual que en Gráficos, usa el selector `Localidad:` si está disponible.

---

## Exportar reportes

En la pestaña **Datos** o **Gráficos**, usa el botón **Exportar PDF** para generar
un reporte de los datos actuales.

---

## Gestión de usuarios (solo admin)

Ve al menú **Usuarios** para crear, editar o desactivar cuentas y asignar roles.

---

## Soporte

¿Problemas? Escribe a **mateo.bha@outlook.com** o abre un
[Issue](https://github.com/mateobha/Mosquito-Data-Management-System-Galapagos/issues).
