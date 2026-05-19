## IaaS, PaaS y SaaS

Son modelos de Cloud Computing que definen **qué tanto administra el proveedor cloud y qué tanto administras tú**.

---

# 1. IaaS — Infrastructure as a Service

Infraestructura como servicio.

El proveedor te da:

- máquinas virtuales,
- red,
- almacenamiento,
- CPU,
- RAM.

Pero tú administras:

- sistema operativo,
- Docker,
- runtime,
- aplicación,
- seguridad del servidor,
- despliegues.

---

## Ejemplo típico

Amazon Elastic Compute Cloud EC2

AWS te entrega una VM Linux vacía.

Tú haces:

```bash id="g63w6l"
sudo apt install java
sudo apt install docker
```

y despliegas tu app.

---

## Analogía

Te alquilan un terreno vacío.

Tú construyes la casa.

---

## Ventajas

- Máximo control.
- Muy flexible.
- Sirve para arquitecturas complejas.

## Desventajas

- Más mantenimiento.
- Más DevOps.
- Más responsabilidad.

---

# 2. PaaS — Platform as a Service

Plataforma como servicio.

El proveedor administra:

- servidores,
- sistema operativo,
- escalado,
- runtime,
- infraestructura.

Tú solo subes tu aplicación.

---

## Ejemplos

- AWS Elastic Beanstalk
- Heroku
- Google App Engine

---

## Ejemplo

Subes:

```text id="c2r8fr"
app.jar
```

y la plataforma:

- instala Java,
- levanta servidores,
- expone puertos,
- escala.

---

## Analogía

Te entregan una casa ya construida.

Solo llevas tus muebles.

---

## Ventajas

- Deploy rápido.
- Menos administración.
- Ideal para productividad.

## Desventajas

- Menos control.
- Menos personalización.
- Puede ser más caro.

---

# 3. SaaS — Software as a Service

Software como servicio.

No administras nada técnico.

Solo usas el software.

---

## Ejemplos

- Google Workspace
- Notion
- Slack Technologies
- Dropbox

---

## Analogía

Vas a un hotel.

Solo usas el servicio.

---

# Comparación rápida

| Modelo | Tú administras | Ejemplo |
| ------ | -------------- | ------- |
| IaaS   | Casi todo      | EC2     |
| PaaS   | Solo tu app    | Heroku  |
| SaaS   | Nada técnico   | Gmail   |

---

# En backend moderno

Muy común:

| Necesidad                  | Modelo |
| -------------------------- | ------ |
| Máximo control             | IaaS   |
| Deploy rápido              | PaaS   |
| Herramientas empresariales | SaaS   |

---

# Docker y Kubernetes

Docker puede correr en:

- IaaS → EC2
- PaaS → Render/Heroku
- CaaS (Containers as a Service) → ECS/Kubernetes

---

# Lo más usado hoy

En empresas modernas:

- EC2 → infraestructura base
- Docker → empaquetado
- Kubernetes/ECS → orquestación
- SaaS → herramientas de negocio

Todo mezclado.

![alt text](image.png)
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
![alt text](image-6.png)
