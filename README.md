# Teams

Este repositorio está preparado para generar un mapa del código con [Graphify](https://github.com/Graphify-Labs/graphify).

## Requisitos

- Python 3.10 o posterior.
- Graphify instalado localmente. La distribución de PyPI se llama `graphifyy`, pero el comando es `graphify`.
- Para usar la skill `/graphify`, instala y abre [Claude Code](https://claude.ai/code).

## Generar el grafo

Desde la raíz del repositorio, instala Graphify y la skill:

```bash
python -m pip install graphifyy
graphify install
```

Luego, en Claude Code, ejecuta:

```text
/graphify .
```

También puedes invocar el CLI directamente:

```bash
graphify .
```

Graphify analizará los archivos compatibles y creará `graphify-out/`, con el informe (`GRAPH_REPORT.md`), el grafo consultable (`graph.json`) y la visualización interactiva (`graph.html`). Para actualizar el grafo después de cambios, vuelve a ejecutar `/graphify . --update` o `graphify . --update`.

## Notas

- La instalación de Graphify es local; no se guardan credenciales ni configuración privada en este repositorio.
- Los artefactos generados por Graphify se excluyen de Git mediante `.gitignore`.
- La documentación oficial y los requisitos pueden cambiar: consulta [Graphify](https://github.com/Graphify-Labs/graphify).
