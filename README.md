# Instagram Backend Microservices

This repository serves as a **monolithic repository** that aggregates multiple backend microservices for the Instagram clone project.  
Each microservice is added as a **Git submodule** for independent development and deployment.

---

## Project Structure
instagram-be-microservices/
├── auth-service/ # Authentication service
├── post-service/ # Post and media service
├── discovery-service/
├── monitor-service/
├── config-server/
├── gateway-server/
├── vault/ Secret service
└── infrastrcuture/

## Getting Started

### 1. Clone the repository with all submodules
```bash
git clone --recurse-submodules https://github.com/DinhXuanLoc2004/instagram-be-microservices.git
```

If you already cloned without --recurse-submodules, run:
```bash
git submodule update --init --recursive
```

### 2. Update submodules
To pull the latest changes from all submodules:
```bash
git submodule update --remote --merge
```

Or update a specific service:
```bash
cd auth-service
git pull origin main
```

Then commit the updated pointer in the main repo:
```bash
cd ..
git auth-service
git commit -m "Update auth service to latest commit"
```

## Notes
    Commit changes inside each microservice in its own repository, then update the pointer here.
    The main repository only tracks submodule commits, not the full history of each service.




