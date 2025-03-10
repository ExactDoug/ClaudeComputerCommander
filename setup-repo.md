# Setup and Push Guide

## Prerequisites
- Git installed and configured
- GitHub CLI (`gh.exe`) installed and authenticated
- Access to the repository fork at `https://github.com/ExactDoug/ClaudeComputerCommander`

## Steps

### 1. Create a New Directory
```powershell
mkdir C:\dev\od-dm-y\OneDrive\dev-projects\mcp\ClaudeComputerCommander
```

### 2. Initialize a Git Repository
```powershell
cd C:\dev\od-dm-y\OneDrive\dev-projects\mcp\ClaudeComputerCommander
git init
```

### 3. Add Remote Repository
```powershell
git remote add origin https://github.com/ExactDoug/ClaudeComputerCommander.git
```

### 4. Fetch Latest Changes
```powershell
git fetch origin
```

### 5. Checkout Main Branch
```powershell
git checkout -t origin/main
```

### 6. Copy Modified Files
```powershell
robocopy "C:\Users\dmortensen\AppData\Local\npm-cache\_npx\e54cca0e4081644e\node_modules\@wonderwhy-er\desktop-commander" "C:\dev\od-dm-y\OneDrive\dev-projects\mcp\ClaudeComputerCommander" /mov
```

### 7. Stage All Changes
```powershell
git add .
```

### 8. Commit Changes
```powershell
git commit -m "Initial commit with local changes"
```

### 9. Push to GitHub Fork
```powershell
git push -u origin main
```

## Notes
- This guide assumes you are using PowerShell on Windows.
- Ensure all commands are run in the correct directory.
- Verify the remote URL and branch names match your repository structure.