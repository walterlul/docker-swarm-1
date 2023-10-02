# DOCKER SWARM

## comandos utilizados en un entorno de Docker Swarm para administrar servicios y despliegues de aplicaciones

### 1 Iniciar docker swarm
docker swarm init

### 2. Desplegar una Pila de Servicios
docker stack deploy -c docker-compose.yml mystack

### 3. Listar servicios
docker service ls

### 4. Ver Detalles de una Instancia de Servicio
docker service ps mystack_web

### 5. Actualizar el Número de Réplicas de un Servicio
docker service update --replicas=5 mystack_web

### 6. Escalar un Servicio
docker service scale mystack_web=5