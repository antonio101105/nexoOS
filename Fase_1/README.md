# 🛠️ Estado del Proyecto: FASE_1

La **FASE_1** de este sistema se ha completado satisfactoriamente. Para garantizar la reproducibilidad y el cumplimiento estricto de los estándares de construcción, todo el proceso se ha realizado de forma automatizada.

### ⚙️ Metodología de Construcción
Se han utilizado exclusivamente los scripts de **jhalfs** (ALFS), los cuales permiten compilar el sistema base extrayendo las instrucciones directamente del libro de *Linux From Scratch*.

* **Herramienta:** [jhalfs (Automated Linux From Scratch)](https://www.linuxfromscratch.org/alfs/)
* **Estado:** `COMPLETADO` ✅
* **Descripción:** Generación automática de los Makefile y ejecución del entorno de compilación para la Fase 1 (herramientas temporales).

> [!IMPORTANT]
> No se realizaron intervenciones manuales en los scripts de compilación durante esta fase para asegurar que el entorno sea 100% fiel a las especificaciones oficiales de LFS.

---

## 🚀 Instrucciones para Reproducir la FASE_1

Si deseas replicar el entorno de construcción exacto utilizado en **El Nexo OS**, sigue estos pasos en tu terminal:

### 1. Descarga el repositorio completo
```bash
git clone https://github.com/antonio101105/nexoOS.git
```
```bash
cd Fase_1
```
```bash
make
```
