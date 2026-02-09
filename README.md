
# witr_AppImage

witr is a CLI utility designed to answer "Why is this running?".

witr tracks processes and their causal ancestry, explaining origins, supervising service, context like directories and containers, risk signals, JSON output, and open ports.

https://github.com/pranshuparmar/witr

## Repository: https://github.com/ryuuzaki42/witr_AppImage
    witr: 0.2.7

## Usage
```
# Base:
    ./witr*_JB-x86_64.AppImage

    # Inspect a running process by name
    ./witr*_JB-x86_64.AppImage nginx

    # Look up a process by PID
    ./witr*_JB-x86_64.AppImage -p 1234

    # Find the process listening on a specific port
    ./witr*_JB-x86_64.AppImage --port 5432

    # Inspect a process by name with exact matching (no fuzzy search)
    ./witr*_JB-x86_64.AppImage bun --exact

    # Show extended process information (memory, I/O, file descriptors)
    ./witr*_JB-x86_64.AppImage mysql --verbose

    # Combine flags: inspect port, show environment variables, output JSON
    ./witr*_JB-x86_64.AppImage --port 8080 --env --json

    # Help and more informations
    ./witr*_JB-x86_64.AppImage -h
```

### Permissions Note
witr inspects system directories which may require elevated permissions.
If you are not seeing the expected information, try running as root.

---
https://github.com/pranshuparmar/witr/releases
