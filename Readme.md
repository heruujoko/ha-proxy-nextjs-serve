# HA-PROXY example for path based routing

## Requirements
- Should have docker and docker-compose available
- node 16

## Run 
- please build each nextjs project with `npm run build`. This step is a requirement for arm based host (Apple Silicon) which has issue with rust dependency on nextjs swc
- on non Apple Silicon host, you can use the same method above or add build step on each Dockerfile
- on the root project run docker compose
- access by http://localhost

## Simulation
- / route should be served by instance ONE and THREE
- /help route should be served only by instance TWO