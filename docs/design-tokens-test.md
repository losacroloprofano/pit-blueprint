# Prueba de Design Tokens (PIT)

Esta página demuestra que `tokens.css` está cargado desde el CDN del Blueprint.

<div class="demo">
  <div class="swatch primary">Primario</div>
  <div class="swatch secondary">Secundario</div>
  <div class="swatch accent">Acento</div>
</div>

<div class="demo">
  <div class="chip">Font base: var(--pit-font-family)</div>
  <div class="chip">Base size: var(--pit-font-size-base)</div>
  <div class="chip">Line height: var(--pit-line-height)</div>
</div>

<style>
/* Esta página asume que tokens.css ya está incluido vía mkdocs.yml -> extra_css */
.demo {
  display: flex; gap: var(--pit-spacing-md); 
  margin: var(--pit-spacing-lg) 0; flex-wrap: wrap;
  font-family: var(--pit-font-family);
}
.swatch {
  padding: var(--pit-spacing-lg);
  color: white;
  border-radius: 12px;
  min-width: 160px; text-align: center;
  box-shadow: 0 6px 18px rgba(0,0,0,.08);
}
.swatch.primary   { background: var(--pit-color-primary); }
.swatch.secondary { background: var(--pit-color-secondary); }
.swatch.accent    { background: var(--pit-color-accent); }
.chip {
  padding: var(--pit-spacing-sm) var(--pit-spacing-md);
  border-radius: 999px;
  background: var(--pit-gray-200);
  color: var(--pit-gray-900);
  border: 1px solid var(--pit-gray-300);
}
</style>

> Si ves tres tarjetas de color y "chips" con tipografía consistente,
> los **tokens** están funcionando ✅.
