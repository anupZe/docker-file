# 🐳 Docker Multi-Stage Build Optimization

## 📌 Project Overview
Optimized Docker images for 4 microservices using multi-stage builds.
Reduced total image size from **~2GB to 24-25MB** (95%+ reduction).

## 🛠️ Services
| Service | Language/Tech | Original Size | Optimized Size |
|---|---|---|---|
| API Service | Node.js | ~400MB | ~8MB |
| Backend Service | Go | ~800MB | ~5MB |
| Database | PostgreSQL | ~400MB | ~6MB |
| Query Service | SQL | ~400MB | ~5MB |

## ⚡ Optimization Techniques Used
- ✅ Multi-stage builds
- ✅ Alpine/Distroless base images
- ✅ Layer caching optimization
- ✅ Removing unnecessary dependencies
- ✅ .dockerignore file

## 📂 Structure
docker-file/
├── nodejs/Dockerfile
├── golang/Dockerfile
├── postgres/Dockerfile
├── sql-service/Dockerfile
└── docker-compose.yml

## 🚀 How to Run
# Clone the repo
git clone https://github.com/anupZe/docker-file

# Run all services
docker-compose up --build

## 📊 Result
Before optimization: ~2GB total
After optimization: ~24MB total
Size reduction: 98.8% 🎯
