# Proceso de configuracion de scheduler para playbook de Monitoreo de Certificados

## Opción recomendada (1 solo schedule)

**Schedule: Diario (ej. 08:00 AM)**

AAP UI

    - Ir a Job Template (cert monitor)
    - Pestaña Schedules → Add
    - Tipo: Recurring
    - Repetition: Daily
    - Hora: 02:00 (lo típico)
    - Timezone: la del cliente (importante)

Por qué diario:

    Detectar el inicio de la ventana “≤ 90 días” inmediatamente.
    Evitar que se “pierda” el primer aviso por calendario.