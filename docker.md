Volume map with bookmark for node_modules: 
  docker run -v /app/node_modules -v $(pwd):/app <container_id>
  docker compose: volumes => - /app/node_modules - .:/app
