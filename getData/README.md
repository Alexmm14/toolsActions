# �Get Data Action

Esta acción procesa la información del commit actual y el repositorio para generar outputs para tus workflows.

## ❤ Inputs

| Nombre | Descripciún | Requerido |
| :--- | :--- | :--- |
| `docker_digest` | Hash de la imagen generada. | No |

## 💔 Ejemplo de uso

```yaml
- name: Extraer Variables
  id: vars
  uses: Alexmm14/toolsActions/getData@master
  with:
    docker_digest: ${{ steps.docker_build.outputs.digest }}
```