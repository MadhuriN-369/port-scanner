# Port Scanner

A simple multi-threaded TCP port scanner written in C++ for Linux systems.

## Features

- Multi-threaded scanning for faster execution
- Scans a user-specified range of ports
- Color-coded terminal output for open and closed ports
- Displays common service names for known ports
- Lightweight implementation using C++ sockets and POSIX threads

## Requirements

- Linux
- g++
- POSIX thread library (`pthread`)

## Build

```bash
g++ portScanner.cpp -o portscanner -pthread
```

## Usage

```bash
sudo ./portscanner
```

Enter the target IP address and port range when prompted.

Example:

```text
Target IP: 192.168.1.1
Start Port: 1
End Port: 1024
```

## Example Output

```text
[OPEN] 22   -> SSH
[OPEN] 80   -> HTTP
[OPEN] 443  -> HTTPS
```

## Future Improvements

- IPv6 support
- Service banner detection
- SYN scanning
- Export scan results to a file
- Custom thread pool implementation

## Disclaimer

This project is intended for educational purposes and authorized security testing only. Do not scan networks or systems without permission.

## License

This project is licensed under the MIT License.
