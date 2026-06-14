# Level Devil — Proyecto Personal

Clon del juego **Level Devil** construido con HTML5 Canvas y vanilla JavaScript, generado con **Aider + Ollama** corriendo localmente en un Mac M3.

---

## ¿Qué es este proyecto?

Level Devil es un *rage platformer* — un juego de plataformas donde el objetivo es simple (llegar a la puerta verde), pero el juego te traiciona constantemente con trampas inesperadas.

Este proyecto es una réplica construida 100% offline usando:
- **Aider** como herramienta de programación con IA
- **Ollama** con el modelo `qwen2.5-coder:14b` corriendo localmente
- **HTML5 Canvas + vanilla JavaScript** — sin librerías externas

---

## Estado actual

### ✅ Fase 1 — Motor base (completado)
- Personaje cuadrado blanco con ojitos que se mueve y salta
- Gravedad y colisiones con plataformas flotantes
- Puerta de salida verde — al tocarla muestra "¡Nivel completado!"
- Game Over al caer fuera del canvas
- Botón de reinicio funcional
- Controles: flechas o A/D para moverse, Espacio/W/↑ para saltar

### 🔄 Fase 2 — Trampas (en progreso)
- [ ] Pinchos que matan al tocarte
- [ ] Hoyos en el suelo que aparecen de sorpresa
- [ ] Plataformas que desaparecen al pisarlas

### 📋 Fase 3 — Troleo real (pendiente)
- [ ] Gravedad invertida sin aviso
- [ ] Controles invertidos (izquierda es derecha)
- [ ] Pinchos que salen de la pared de sorpresa
- [ ] Plataformas falsas (parecen sólidas pero no lo son)

---

## Cómo correrlo

No necesitas instalar nada. Solo abre el archivo en tu navegador:

```bash
open leveldevil.html
```

---

## Cómo desarrollarlo con Aider

### Requisitos
- [Ollama](https://ollama.com/download) instalado
- Aider instalado (`pip3 install aider-chat`)
- Modelo descargado: `ollama pull qwen2.5-coder:14b`

### Iniciar sesión de desarrollo

```bash
# Terminal 1 — iniciar Ollama
ollama serve

# Terminal 2 — iniciar Aider
export OLLAMA_API_BASE=http://localhost:11434
cd ~/Desktop/proyectogame
aider --model ollama/qwen2.5-coder:14b leveldevil.html
```

---

## Aprendizajes del proceso

- Las instrucciones **muy específicas y detalladas** dan mejores resultados con Aider
- Mejor construir en fases pequeñas que pedir todo de una vez
- El modelo `qwen2.5-coder:14b` es el más confiable para código en este setup
- Siempre recargar el navegador con `Cmd + R` después de cada cambio

---

## Controles del juego

| Tecla | Acción |
|---|---|
| `A` / `←` | Mover izquierda |
| `D` / `→` | Mover derecha |
| `W` / `↑` / `Espacio` | Saltar |

---

*Proyecto de aprendizaje — Junio 2026*
