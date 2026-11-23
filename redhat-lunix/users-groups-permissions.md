# Red Hat Linux Lab

## Objective
Create users, groups and a shared directory for the IT team.

## Users and Group
- Users: ahmed and sara
- Group: IT

## Create Users and Group

```bash
sudo groupadd IT
sudo useradd ahmed
sudo useradd sara
sudo usermod -aG IT ahmed
sudo usermod -aG IT sara
```

## Create Shared Directory

```bash
sudo mkdir -p /company/IT
sudo chown root:IT /company/IT
sudo chmod 770 /company/IT
```

## Permissions
Directory permissions: `drwxrwx---`

- Owner: root
- Group: IT
- Owner and group: full access
- Others: no access

## Test
Both users successfully accessed `/company/IT` and created their files:
- ahmed.txt
- sara.txt

## Skills
- Linux users and groups
- Shared directories
- chmod and chown
- File permissions
