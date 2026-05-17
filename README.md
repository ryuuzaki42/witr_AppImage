
# witr_AppImage

witr is a CLI utility designed to answer "Why is this running?"

witr tracks processes and their causal ancestry, explaining origins, supervising service, context like directories and containers, risk signals, JSON output, and open ports

https://github.com/pranshuparmar/witr

## Repository: https://github.com/ryuuzaki42/witr_AppImage
    witr: 0.3.2

## Usage
```
# Base
    ./witr-*_JB-x86_64.AppImage

# Inspect a running process by name
    ./witr-*_JB-x86_64.AppImage nginx

# Look up a process by PID
    ./witr-*_JB-x86_64.AppImage -p 1234

# Find the process listening on a specific port
    ./witr-*_JB-x86_64.AppImage --port 5432

# Inspect a process by name with exact matching (no fuzzy search)
    ./witr-*_JB-x86_64.AppImage bun --exact

# Show extended process information (memory, I/O, file descriptors)
    ./witr-*_JB-x86_64.AppImage mysql --verbose

# Combine flags: inspect port, show environment variables, output JSON
    ./witr-*_JB-x86_64.AppImage --port 8080 --env --json

# Help
    ./witr-*_JB-x86_64.AppImage -h
```
### Permissions note
witr inspects system directories which may require elevated permissions
If you are not seeing the expected information, try running as root

### Run it as root
    su
    ./witr-*_JB-x86_64.AppImage

### Or
    sudo ./witr-*_JB-x86_64.AppImage

### If use KDE
    kdesu ./witr-*_JB-x86_64.AppImage

---
https://github.com/pranshuparmar/witr/releases
