# Discovery Agent

## Estructura

```text
discovery-agent/
├── .claude/
│   └── scripts/
├── .idea/
├── discoveries/
│   ├── _template/
│   │   ├── interviews/
│   │   └── outputs/
│   └── citasalud/
│       ├── interviews/
│       └── outputs/
├── CLAUDE.md
└── README.md
```

## Reglas de trabajo (no negociables)

- Todo discovery vive dentro de `discoveries/<nombre>/`.
- Cada discovery separa entrevistas en `interviews/` y entregables en `outputs/`.
- No mezclar notas crudas, entrevistas y conclusiones finales en el mismo archivo.
- Usar `_template/` como referencia para crear nuevos discoveries.

## Flujo de trabajo

1. Crear una carpeta nueva en `discoveries/<nombre>/`.
2. Crear sus subcarpetas `interviews/` y `outputs/`.
3. Guardar entrevistas, transcripciones o notas crudas en `interviews/`.
4. Generar hallazgos, resúmenes, reportes o artefactos finales en `outputs/`.
5. Mantener `README.md` actualizado con el objetivo general del repositorio.

## Los gates (reglas duras, por discovery)

- `interviews/` debe contener la evidencia o material fuente.
- `outputs/` debe contener solamente resultados listos para revisar o compartir.
- Todo output importante debe poder rastrearse a entrevistas o notas fuente.
- Antes de cerrar un discovery, revisar que no haya archivos finales fuera de `outputs/`.
