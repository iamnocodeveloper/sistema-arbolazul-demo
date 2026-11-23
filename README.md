# Centro Infantil El Árbol Azul — demo del sistema de gestión

Demo navegable (una sola página, sin backend) del sistema de gestión para el
**Centro Infantil El Árbol Azul** (Costa Rica), un centro infantil / jardín maternal
que trabaja por salas según la edad.

## Qué muestra

- **Entrada**: botón «Entrar al sistema» y «Ver el recorrido guiado».
- **Panel del día**: solicitudes nuevas, matrículas por confirmar, pagos de la semana
  (al día / por vencer / vencidos), asistencia de hoy y avisos por enviar a los padres.
- **Inscripciones**: embudo y tabla con buscador y estados
  (nueva · contactada · visita agendada · admitida · matriculada · lista de espera) y ficha
  del niño con edad, sala por edad, quién lo inscribe, alergias u observaciones,
  documentos entregados y descuento por hermanos.
- **Pagos y mensualidades**: estado de cada mensualidad, botón «Enviar recordatorio por
  WhatsApp» que abre el chat de la familia con el mensaje armado y el aviso automático
  del sistema 5 días antes del vencimiento.
- **Asistencia**: pase de lista por sala (presente/ausente) y aviso a la familia cuando el
  niño no llegó.
- **Comunicados**: aviso general a una sala o a la familia de un niño, con maqueta del
  mensaje de WhatsApp e historial.
- **Informes**: gráficos propios (SVG/CSS) de solicitudes por mes, matriculados por sala,
  cobrado vs. pendiente y asistencia promedio.
- **Web pública**: presentación del centro con las salas por edad, el horario real
  (lunes a viernes de 6:00 a.m. a 6:00 p.m.), qué incluye el día, aviso de lista de espera y
  formulario «Solicitar informes / pre-inscripción» que arma el mensaje de WhatsApp al
  **+506 8392 3872**.
- **Recorrido guiado**: tour de 7 pasos sobre la interfaz, con Atrás / Siguiente / Salir,
  contador de paso, teclado (← → Esc) y modo automático.

## Datos

Todos los datos (nombres, edades y montos) son **de ejemplo**. Los montos se muestran en
colones solo como referencia o como «Consultar». No se envía ni se guarda nada: la app es
estática y no realiza ninguna petición al abrir los enlaces de WhatsApp.

## Ejecutar

```bash
docker build -t sistema-arbolazul .
docker run -p 8080:80 sistema-arbolazul
```

---

Demo de referencia hecho por **Nocodeveloper**. Los datos son de ejemplo.
