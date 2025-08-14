# Log Archive Utility

A simple Python script to archive log directories into compressed `.tar.gz` files with timestamped filenames.

## Features

- Creates compressed archives of log directories
- Generates timestamped archive filenames
- Maintains a log of all archive operations
- Creates an `archives` directory automatically
- Simple command-line interface

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

```bash
./log-archive.py <log-directory>
```

Or using Python directly:

```bash
python3 log-archive.py <log-directory>
```

### Example

```bash
./log-archive.py /var/log/myapp
```

This will create:
- A compressed archive in `./archives/logs_archive_YYYYMMDD_HHMMSS.tar.gz`
- An entry in `./archives/archive_log.txt`

## Output Structure

The script creates:
```
./
└── archives/
    ├── logs_archive_YYYYMMDD_HHMMSS.tar.gz
    ├── logs_archive_... (previous archives)
    └── archive_log.txt (log of all archive operations)
```

## License

[MIT License](LICENSE)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author

[kunal-1207](https://github.com/kunal-1207)
https://roadmap.sh/projects/log-archive-tool
