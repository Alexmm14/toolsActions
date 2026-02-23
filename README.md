# 🙻 Alexmm14 Tools Actions

Este repositorio centraliza las **GitHub Composite Actions** utilizadas para estandarizar el flujo de trabajo en múltiples proyectos.

## 𝐃 Estructura del Repositorio

* **/getData**: Extrae información del contexto de Git y del repositorio.
* **/notify-n8n**: Acción genérica para enviar webhooks JSON dinámicos.

## 🚀 Uso General

Para utilizar cualquiera de estas acciones, es requerido incluir el paso de checkout con hetch-depth: 0:

```yaml
steps:
  - name: Checkout
    uses: actions/checkout@v4
    with:
      fetch-depth: 0

  - name: Extraer Datos
    uses: Alexmm14/toolsActions/getData@master
```

---
MIT License © 2026 Alexmm14