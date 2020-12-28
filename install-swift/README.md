# Installing Swift Programming Language

### Adding Swift ARM Repository
```
curl -s https://packagecloud.io/install/repositories/swift-arm/release/script.deb.sh | sudo bash
```
### Install Swift5
```
sudo apt-get update
sudo apt-get install swift5

# Check if installed properly
swift --version
```

### Compile and Run Test Project

```
# Create Project Directory
mkdir TestProject
cd TestProject

# Create Empty Project
swift package init --type=executable

# Compile and Run Test Project
swift run
```



