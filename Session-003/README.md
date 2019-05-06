# Session-3:

### 1. Dockerize
- Everybody should dockerize a project[Moein, Yasin]
- Project should be based on Node but serve with nginx
- Docker multi staging [here](https://docs.docker.com/develop/develop-images/multistage-build/)

---
**Example:**
```bash
From node:latest as builder 
...

From nginx:latest
...
```

