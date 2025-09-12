# 🚀 Hello World!!! 

A simple **HELLO WORLD** program to run on CleanStart - Step CLI container. 

## To run the Hello World without Dockerfile to avoid making simple things complex

### Pull CleanStart Step CLI image from [Docker Hub - CleanStart](https://hub.docker.com/u/cleanstart) 
```bash
docker pull cleanstart/step-cli:latest
```
```bash
docker pull cleanstart/step-cli:latest-dev
```

## If you have the Step CLI image pulled, you can also run your program directly:
```bash
docker run --rm -v $(pwd):/app -w /app cleanstart/step-cli:latest python hello_world.py
```
## Output 
```bash
============================================================
🔐 Step CLI - Hello World
============================================================
Timestamp: 2024-01-15 10:30:45
Python Version: 3.11.0 (main, Oct 24 2023, 00:00:00) [GCC 11.2.0]
Working Directory: /app
============================================================

🔍 Checking Environment...
✅ Running in Docker container
✅ Step CLI is available
   Version: Smallstep CLI/0.24.4 (linux/amd64)
✅ Step CA is available
   Version: Smallstep CA/0.24.4 (linux/amd64)

🧪 Testing Step CLI...
✅ Step CLI version check passed
✅ Step CA version check passed
✅ Certificate generation test passed

📋 Sample Step CLI Commands:
----------------------------------------
   Check version:
     step version

   Initialize CA:
     step ca init

   Generate certificate:
     step certificate create test-cert test.crt test.key

   Inspect certificate:
     step certificate inspect test.crt

============================================================
🎉 Step CLI Hello World completed!
============================================================
```

## 📚 Resources

- [Verified Docker Image Publisher - CleanStart](https://cleanstart.com/)
- [Step CLI Documentation](https://smallstep.com/docs/step-cli/)

## 🤝 Contributing

Feel free to contribute to this project by:
- Reporting bugs
- Suggesting new features
- Submitting pull requests
- Improving documentation

## 📄 License
This project is open source and available under the [MIT License](LICENSE).