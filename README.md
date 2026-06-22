# UdeSA — Modelado Estocástico (MIA103)

Notebooks de la materia. Para ejecutarlos localmente conviene usar un entorno virtual (`.venv`) con las dependencias listadas en [requirements.txt](requirements.txt).

## Requisitos

- Python 3.10 o superior
- VSCode con la extensión de Jupyter (para correr los `.ipynb`)

## Entorno virtual (`.venv`)

> Los comandos asumen que estás parado en la raíz del repositorio.

### Crear el entorno

```powershell
python -m venv .venv
```

### Activar el entorno

**Windows — PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

> Si PowerShell bloquea el script con un error de *ExecutionPolicy*, ejecutá una vez:
> ```powershell
> Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
> ```

**Windows — CMD:**

```cmd
.\.venv\Scripts\activate.bat
```

**Linux / macOS:**

```bash
source .venv/bin/activate
```

Con el entorno activo, el prompt muestra el prefijo `(.venv)`.

### Instalar las dependencias

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Desactivar el entorno

```powershell
deactivate
```

### Eliminar el entorno

Primero desactivalo (`deactivate`) y luego borrá la carpeta `.venv`.

**Windows — PowerShell:**

```powershell
Remove-Item -Recurse -Force .venv
```

**Linux / macOS:**

```bash
rm -rf .venv
```

## Ejecutar los notebooks en VSCode

1. Abrí un notebook (`.ipynb`).
2. En la esquina superior derecha, hacé clic en **Select Kernel**.
3. Elegí el intérprete de Python del entorno `.venv`.
