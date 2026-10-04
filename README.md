# catall

A minimal terminal command that displays the contents of files in the current directory while keeping folders and binary files visually distinct.

## Features

- Displays folders without entering them
- Displays printable file contents
- Displays binary files without dumping their contents
- `--hidden` flag to include hidden files
- Clean terminal output with color-coded file types
- No recursive traversal
- No dependencies

## Installation

Clone the repository:

```bash
git clone https://github.com/thearkabanerjee/catall.git
cd catall
```

Make the command executable:
```bash
chmod +x catall
```

Move it somewhere in your PATH:
```bash
mkdir -p ~/.local/bin
mv catall ~/.local/bin/
```

If ~/.local/bin is not already in your PATH (just make it):
```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

You can now use catall from any directory:
```bash
catall
```

### Requirements
- macOS or Linux
- Bash
- file
No additional packages or dependencies are required.

### Design
catall is intentionally simple.
It only operates on the current directory and does not recursively enter folders. This keeps the output compact and makes it useful for quickly inspecting a project or directory.

### Display visible files and folders.
```bash
catall --hidden
```

### License
MIT License
