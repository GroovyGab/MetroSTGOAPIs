# MetroSTGOAPIs

Este repositorio está dedicado a proveer acceso a las diversas APIs que usa Metro de Santiago (Principalmente en la app móvil) para dar información acerca del estado de la red de transporte e información miscelánea.

- Estado general de la red: GET https://www.metro.cl/api/estadoRedDetalle.php
  
- Tarifas: GET https://www.metro.cl/api/tarifario.php
  
- Planificador de rutas: GET https://www.metro.cl/api/planificadorv2.php?estacionInicio={*CÓDIGO_ESTACIÓN_INICIAL}&estacionFin={*CÓDIGO_ESTACIÓN_FINAL}&dia=dl&hora={*HORARIO}
  
- Información especifica acerca de una estación: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/informacion/{*CÓDIGO_DE_ESTACIÓN}
  
- Información especifica a Metroarte de una estación: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/metroarte?estacion={*CÓDIGO_DE_ESTACIÓN} (Requiere que el header "User-Agent" esté presente en la petición o la página responderá con 403 Forbbiden)
  
- Información sobre rutas expresas: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/ruta
  
- Plano de la red de Metro: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/planored
  
- Información detallada sobre las tarifas: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/tarifario/{HorarioBajo/HorarioValle/HorarioPunta}
  
- Agenda cultural: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/agendacultural
  
- Proyectos: GET https://8pt7kdrkb0.execute-api.us-east-1.amazonaws.com/UAT/proyectos/{*NÚMERO_DE_LINEA}
