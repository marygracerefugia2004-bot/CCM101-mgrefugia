# Firewall Configuration

## 1. Allow SSH

**Question: What command was used to allow SSH?**

**Answer:**

```bash
sudo ufw allow ssh
```

This command allows SSH traffic so administrators can remotely manage the server.

## 2. Set the Default Deny Policy

**Question: What commands were used to set the Default Deny policy?**

**Answer:**

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming traffic unless a rule allows it, while the second allows outgoing traffic by default.

## 3. Enable the Firewall

**Command used:**

```bash
sudo ufw enable
sudo ufw status verbose
```

These commands activate UFW and display its status and default policies.

## 4. Allow Port 8080

**Question: What command was used to allow Port 8080?**

**Answer:**

```bash
sudo ufw allow 8080/tcp
```

This command allows TCP traffic on port 8080 for the web application used in this activity.

To verify the numbered firewall rules, I used:

```bash
sudo ufw status numbered
```

## 5. Test the Web Application

**Command used:**

```bash
curl http://localhost:8080
```

This command sends a request to the local web application to check whether it responds.

## 6. SSH Security Warning

**Question: What would happen if you ran `sudo ufw enable` before running `sudo ufw allow ssh`?**

**Answer:**

Enabling the firewall before allowing SSH could block remote SSH connections under the default deny policy, potentially locking the administrator out of the server.
