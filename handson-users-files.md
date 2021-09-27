# Create userA and userB and check if the users created
- useradd [OPTIONS] USERNAME
- useradd creates a new user account according to the options specified on the command line and the default values set in the /etc/default/useradd
- The command adds an entry to the /etc/passwd, /etc/shadow, /etc/group and /etc/gshadow files
- only sudo users can create
```bash
sudo useradd userA
sudo useradd userB
sudo cat /etc/passwd
```

# Give userA admin rights
- With the new user created, it's time to give them sudo rights. For this we'll use the usermod command like so:
```bash
sudo usermod -aG sudo userA
```

# Create /operations folder
```bash
cd /
mkdir operations
```
# User A must have admin rights on /operations
