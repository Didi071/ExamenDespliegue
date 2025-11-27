# Uso de Git

## Instalacion

El git init para crear el repo local. Luego lo añades al remoto con git remote add urlDelRepo

## Configuración

Se hace con las variables globales

### Comandos clave:

```bash
git config --global user.name "Diana"
git config --global user.email "diana@example.com"
git config --global core.editor "code --wait"   # VS Code como editor
git config --global color.ui true               # Colores bonitos
git config --global core.autocrlf true          # Manejo de saltos de línea
```

## GitFlow

1. Rama Main (no se toca)
2. Rama Develop (principal de desarrollo)
3. Rama Feature (para desarrollar partes especificas)
4. Rama Release (la de las pruebas unitarias. Paso previo para mergear con main)
5. Rama Hotfix (errores reapidos se mergea directamente a main)

---

### Crear o clonar repos

```bash
git init
git clone <url>
```

---

### 4. Workflow diario

```bash
git status
git add archivo
git add .
git commit -m "mensaje"
git push origin main
git pull
```

Diferencias y log:

```bash
git diff
git diff --staged
git log --oneline --graph
```

Restaurar:

```bash
git restore archivo
```

## 5. Comandos

Crear / cambiar:

```bash
git switch -c nueva-rama
git switch rama
```

Borrar:

```bash
git branch -d rama
```

**Merge** (une ramas):

```bash
git switch main
git merge mi-rama
```
