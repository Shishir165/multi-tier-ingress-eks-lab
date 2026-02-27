# Multi-Tier App on EKS with CI/CD

## 🚀 Live URL
http://shishirp.diogohack.shop

---

## 🏗 Architecture

- EKS Cluster (us-east-1)
- Traefik Ingress Controller
- Backend (Node.js)
- Frontend
- Docker Hub (image registry)
- GitHub Actions (CI/CD)

---

## 🔁 CI/CD Flow

On every push to `main`:

1. Build backend Docker image
2. Build frontend Docker image
3. Push images to Docker Hub
4. Deploy updated images to EKS
5. Run smoke test

No manual kubectl required.

---

## 🧪 Test Endpoint

```bash
curl http://shishirp.diogohack.shop/api/ping

📦 Docker Images

shishir165/lab-backend

shishir165/lab-frontend

✅ Status

CI/CD pipeline successfully deployed via GitHub Actions.