# 🧰 Odoo Product Images

Repositorio público destinado a alojar las **imágenes de productos** utilizadas en la carga masiva y gestión visual dentro de **Odoo** (Inventario, eCommerce y Punto de Venta).

---

## 📦 Propósito

Este repositorio funciona como una **fuente estática (CDN público)** para vincular imágenes mediante **URLs directas (RAW)** desde GitHub.

Estas direcciones pueden utilizarse al importar productos en Odoo, dentro del campo:
```
image_1920
```

---

## 🗂️ Estructura del repositorio

```
/fotos/
├── freno_hyundai.jpg
├── bandeja_corsa.png
├── bujia_ngk.jpg
└── ...
```

---

## 🔗 Cómo obtener la URL pública de una imagen

1. Abre la imagen desde la carpeta `/fotos/`.
2. Haz clic en **“View raw”**.
3. Copia el enlace del navegador; tendrá una forma como esta:

```
https://raw.githubusercontent.com/vircof/odoo-product-images/main/fotos/freno_hyundai.jpg
```

4. Pega ese enlace en tu archivo Excel, en la columna `image_1920`.

---

## 💡 Recomendaciones

- Usa nombres simples y sin espacios (`freno_hyundai.jpg` ✅, `Freno Hyundai.jpg` ❌).
- Mantén las imágenes optimizadas (≤1 MB) para evitar lentitud al importar.
- Si reemplazas una imagen, conserva el mismo nombre de archivo para mantener la URL activa.
- Las imágenes deben ubicarse dentro de la carpeta `/fotos/`.

---

## ⚙️ Ejemplo de uso en importación Odoo

| Producto | Código | image_1920 |
|-----------|---------|------------|
| Freno Hyundai | FHY01 | https://raw.githubusercontent.com/vircof/odoo-product-images/main/fotos/freno_hyundai.jpg |
| Bandeja Corsa | BCN02 | https://raw.githubusercontent.com/vircof/odoo-product-images/main/fotos/bandeja_corsa.png |

Luego importa el Excel en  
**Inventario → Productos → Favoritos → Importar registros**  
y Odoo asociará automáticamente las imágenes.

---

## 📍 Contexto

Repositorio auxiliar creado para **MOM**.  
Autor: *Matías Sepúlveda (Vircof)*  
Año: 2025  
Uso: carga masiva y centralizada de imágenes de producto en Odoo.

---

> 💾 Este repositorio no contiene datos sensibles ni código ejecutable.  
> Solo recursos gráficos públicos destinados a integraciones con Odoo.