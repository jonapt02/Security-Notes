# CIA Triad

## ¿Qué es?

En términos generales, **CIA** (o **CID** en español) son las siglas de los tres pilares más importantes de la ciberseguridad.

### Confidencialidad

Se refiere a que los datos de, por ejemplo, una aplicación, sean accesibles únicamente por los usuarios autorizados. Es decir, la información de nivel administrativo solo debe estar disponible para usuarios con privilegios administrativos, mientras que los datos personales únicamente deben ser accesibles para su propietario, y así sucesivamente.

Así como en una cocina, el cliente no debería conocer la receta del chef porque solo él la sabe; de la misma manera, el chef no debería conocer cuánto dinero tiene el cliente.

### Integridad

Esta parte hace referencia a que ninguna persona sin autorización pueda modificar datos fuera de los permisos que tiene asignados. Está claramente ligada a la confidencialidad, pero no es lo mismo, ya que nos lleva a pensar en cómo evitar, a toda costa, que un usuario externo o sin privilegios en la aplicación o en la base de datos pueda modificar información existente sin la autorización correspondiente.

Siguiendo el ejemplo de la cocina, ningún cliente debería tener acceso para modificar la receta del chef, ni el chef debería poder modificar aspectos de la vida del cliente.

### Disponibilidad

Creo que esta es la más clara y complementa los principios de confidencialidad e integridad, ya que, básicamente, establece que los datos deben estar siempre disponibles cuando sean necesarios, gracias a que son confidenciales y no han sido modificados de manera indebida.

Siguiendo el ejemplo de la cocina, sería como un restaurante que permanece abierto para atender a sus clientes cada vez que lo requieran, algo similar a un restaurante que opera las 24 horas del día. Depende de la administración del restaurante garantizar que pueda operar de forma continua.


## Resumen

| Pilar | Objetivo |
|--------|----------|
| Confidencialidad | Evitar accesos no autorizados. |
| Integridad | Evitar modificaciones indebidas. |
| Disponibilidad | Garantizar acceso cuando sea necesario. |


Desde la perspectiva de una persona enfocada a BLUE TEAM esto implicaría lo siguiente:

- Estar constantemente reglas de acceso
- Motinatoreando constantemente el sistema para ver quien accede  buscando 
- Anomalias en las modificaciones a los datos 
- Supervisando constantemente a diponibilidad del sistema

## Herramientas relacionadas

- Wazuh
- Active Directory
- Sysmon
- Linux

## Ataques relacionados

Confidencialidad

- Credential Dumping
- Phishing

Integridad

- SQL Injection
- Data Tampering

Disponibilidad

- DDoS
- Ransomware