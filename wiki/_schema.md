# Cómo se escribe este wiki

Esta es la parte fija del sistema. Las carpetas cambian según quién lo use; estas reglas no.

## Las seis reglas

1. **Una cosa = una página.** Una jugadora, un cliente, un proveedor, un evento. Nunca una
   página con una lista de cosas adentro.
2. **Si A menciona a B, B menciona a A.** Los enlaces van en los dos sentidos.
3. **Toda página cierra con `## Enlaces`** y enlaces a las páginas relacionadas. Sin eso el
   mapa de Obsidian sale desconectado y no sirve de nada.
4. **Formato de enlace:** `[[carpeta/pagina|Nombre visible]]` — por ejemplo
   `[[equipo/maria-gomez|María Gómez]]`.
5. **Estados:** `ACTIVO`, `PAUSADO`, `TERMINADO`, `CANCELADO`.
6. **Nombres de archivo** en minúsculas, sin acentos ni espacios: `maria-gomez.md`.

## Cuando algo cambia

Tres pasos, siempre los tres:

1. Actualizar la página
2. Actualizar `_index.md` si se creó o se borró una página
3. Añadir una línea a `_log.md`

## Las carpetas fijas

```
wiki/
  _plan.md      la meta y en qué anda
  _index.md     todas las páginas
  _log.md       qué cambió y cuándo
  _schema.md    esto
  assets/       PDFs, imágenes, documentos (solo lectura)
  raw/          Excel, exports, listas viejas (solo lectura)
```

Todo lo demás se crea según el caso.

## Plantillas

### `_plan.md`

```
# {Nombre} — Plan

*Actualizado: AAAA-MM-DD*

## Meta
Una sola frase.

## Ahora
Lo que está activo esta semana.

## Números
Lo que se mide, si se mide algo.

## Parqueado
Lo que no se está haciendo, y por qué.
```

### Una página de persona

```
# {Nombre}

**Estado:** ACTIVO
**Desde:** AAAA-MM-DD

## Situación
Dónde está parado hoy.

## Historial
- AAAA-MM-DD: qué pasó

## Enlaces
- [[carpeta/pagina|Nombre]]
```

### Una página de evento

```
# {Evento}

**Estado:** ACTIVO
**Cuándo:** AAAA-MM-DD, HH:MM
**Dónde:**

## Qué hay que preparar
- ...

## Después
Qué pasó, qué aprendimos.

## Enlaces
- [[carpeta/pagina|Nombre]]
```

### Una página de cosa o recurso

```
# {Cosa}

**Estado:** ACTIVO
**Para qué sirve:**

## Detalles
Lo que hay que recordar.

## Enlaces
- [[carpeta/pagina|Nombre]]
```

### `assets/_catalogo.md`

```
| Archivo | Tipo | Qué es | Añadido |
|---------|------|--------|---------|
```

## Lo que no se hace

- Páginas de relleno "por si acaso"
- Secciones vacías con un guion adentro
- Inventar datos que la persona no dijo — si falta algo, se pregunta
- Tocar `raw/` o `assets/`
