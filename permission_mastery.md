# File Permissions Mastery

## Permission Numbers I've Learned
- **755** = rwxr-xr-x (scripts, executables)
- **644** = rw-r--r-- (documents, text files) 
- **600** = rw------- (private files, secrets)
- **740** = rwxr----- (owner full, group read only)
- **700** = rwx------ (owner only access)

## Real Commands I Used
```bash
chmod 755 script.sh      # Make executable
chmod 644 document.txt   # Standard file
chmod 600 private.txt    # Owner only
