## Common `.gitignore` Patterns

This section provides common `.gitignore` patterns to help keep your repository clean and free of unnecessary files. These patterns cover plaintext files, IDEs and editors, Python, and Terraform, tailored for a general programming setup.

### Plaintext and Sensitive Files

Use these patterns to ignore log files, temporary files, and sensitive files:

```plaintext
# Logs and temporary files
*.log               # Ignore all log files
*.tmp               # Ignore all temp files
*.bak               # Ignore all backup files

# Secrets and environment variables
.env                # Environment variables file
*.key               # Private key files
*.pem               # PEM files (e.g., for SSH keys)
*.csv               # CSV files (adjust if used for sensitive data)
```
# JetBrains IDEs (e.g., PyCharm, IntelliJ)
```plaintext
.idea/              # JetBrains project settings folder
*.iml               # JetBrains module files
```

### Visual Studio Code
```plaintext
.vscode/            # VS Code settings folder
```


### Virtual Environments
```plaintext
env/                # Virtual environment folder
venv/               # Alternate virtual environment folder
.venv/              # Another virtual environment name
```

# Python-specific files
```plaintext
*.pyo               # Optimized Python files
*.pyd               # Windows DLL files for Python modules
*.pdb               # Python debugger files
*.log               # Python log files
```

# Terraform State files
```plaintext
*.tfstate           # State files for resource tracking
*.tfstate.*         # Backup state files

### Terraform variable files (can contain sensitive data)
*.tfvars            # Variable files with sensitive information

### Terraform directories
.terraform/         # Terraform cache and plugin folder

### Crash and backup logs
crash.log           # Crash log files
*.backup            # Terraform backup files
override.tf         # Local override files
override.tf.json    # Local override JSON files
terraform.tfvars    # Terraform variable files with sensitive data
terraform.tfvars.json # JSON variable files with sensitive data
```