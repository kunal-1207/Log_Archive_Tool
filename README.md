# Log Archive Utility

A simple Python script to archive log directories into compressed `.tar.gz` files with timestamped filenames.

[![Project Roadmap](https://img.shields.io/badge/Roadmap-View%20Project%20Plans-blue)](https://roadmap.sh/projects/log-archive-tool)

## Features

- Creates compressed archives of log directories
- Generates timestamped archive filenames (YYYYMMDD_HHMMSS format)
- Maintains a log of all archive operations in `archive_log.txt`
- Automatically creates an `archives` directory if missing
- Simple command-line interface
- Zero external dependencies

## Requirements

- Python 3.6 or higher
- Standard Python libraries (no external dependencies)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/log-archive.git
   ```
2. Navigate to the project directory:
   ```bash
   cd log-archive
   ```
3. Make the script executable (optional):
   ```bash
   chmod +x log-archive.py
   ```

## Usage

Basic command:
```bash
./log-archive.py <log-directory>
```

Alternative using Python directly:
```bash
python3 log-archive.py <log-directory>
```

### Example
```bash
./log-archive.py /var/log/myapp
```

This will create:
- A compressed archive: `./archives/logs_archive_YYYYMMDD_HHMMSS.tar.gz`
- An entry in the operation log: `./archives/archive_log.txt`

## Project Roadmap

For future plans and development priorities, see our [public roadmap](https://roadmap.sh/projects/log-archive-tool).

Current planned improvements include:
- Support for multiple compression formats
- Retention policy configuration
- Remote storage options
- Email notifications

## Output Structure

```
./
└── archives/
    ├── logs_archive_*.tar.gz      # Timestamped archives
    └── archive_log.txt            # Operation history
```

## Contributing

We welcome contributions! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

For major changes, please open an issue first to discuss your proposed changes.

## License

[MIT License](LICENSE)

