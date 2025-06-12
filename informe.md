#  Contenerización React + API

## Proyecto: Dispositivo Guardián Inteligente para Regletas Eléctricas

### Entidad visualizada: `EventosDeSobrecarga`

Este proyecto permite visualizar eventos registrados por un dispositivo inteligente que monitorea el estado de una regleta eléctrica, enfocado en detectar y alertar sobre posibles sobrecargas eléctricas. La entidad principal visualizada es `EventosDeSobrecarga`, cuyos campos son:

- `fecha_hora`: Fecha y hora del evento.
- `voltaje`: Nivel de voltaje registrado en el momento.
- `corriente`: Intensidad de corriente medida.
- `estado`: Estado de la regleta (normal o sobrecarga).

---

### Tecnologías utilizadas

- **Frontend**: React (Create React App)
- **Backend**: Node.js + Express + PostgreSQL
- **Contenerización**: Docker + Docker Compose
- **Comunicación HTTP**: Axios para el consumo del API REST
- **Puerto del backend**: `3001`
- **Puerto del frontend**: `3000`

---

### Comunicación entre contenedores

La comunicación entre los contenedores del frontend y backend se logra usando **Docker Compose**, que crea una red interna para que los servicios se reconozcan por nombre.  
El frontend utiliza la variable de entorno `REACT_APP_API_URL` para comunicarse con el backend a través del hostname `backend`, como se define en `docker-compose.yml`.

### Lo que aprendí
- Cómo contenerizar React y Express.
- Cómo conectar dos contenedores mediante Docker Compose.
- Cómo manejar variables de entorno en React.





