# DOSW_ParcialT1_PedroAyala

### 1. diagrama de contexto
![diagrama de contexto](../DOSW-ParcialT1/docs/images/context.png)

### 2. requerimientos

funcionales:

1. el sistema debe notificar a los estudiantes antes de sus tutorias

2. el sistema debe poder permitir discriminar entre tutores profesores y estudiantes

3. el sistema debe permitir que al momento de generar una reserva darle  un tiempo determinado y cambiar la dinamica dependiendo en ambos casos si es profesor o estudiante

no funcionales

1. debe poner adapatarse entre dispositivos celulares y de escritorio

2. debe tener los colores de la universidad y debe cumplir los estandares minimos de WCAG 2.1 Nivel AA



| Campo | Descripción |
|------|-------------|
| **ID** | RF-03 |
| **Nombre del requerimiento** | GENERACION DE RESERVA |
| **Descripción** | El sistema debe poder al momento de generar una reserva asignarle automaticamente un tiempo maximo dependiendo de si el tutor es profesor o estudiante ademas de cambiar la dinamica d ela tutoria ya que si es estudiante puede explicar no solo materias en especifico sino tambien de temas generales del programa academico . |
| **Precondiciones** | Para que el sistema cumpla con este requerimiento, TutoECI debe tener previamente un organizador que peuda discriminar entre profesores y estudiantes y con sus respetivos permisos activos |
| **Actor** | solicitante  |
| **Flujo principal** | 1. El solicitante inicia sesión en el sistema con sus credenciales.<br>2. el sistema verifica mandandole a enlace el id del estudiante para ver si puede recibir esa tutoria, en caso de que no aqui acabaria el flujo (FASTEST_AVAILABLE,EXPERT_FIRST,PEER_TUTORING).<br>3. El solicitante solicita una tutoria entre 3 opciones <br>4.  El organizador debe descriminar dependiendo de la opcion que el estudiante haya escogido y asignarle un tutor.<br>6. el sistema ya con el tutor asignado debe poder crearle una reserva al estudiante y al profesor <br>7. El sistema notifica a ambos de que se genero una reserva. |
| **Diagrama de caso de uso** | ![Diagrama de caso de uso - Generacion de reserva](../DOSW-ParcialT1//docs/images/diagrama_caso1.png) |
| **Poscondiciones** | Se espera como resultado que la reserva se haya creado actualizando el calendario y horario del profesor y estudiante. |