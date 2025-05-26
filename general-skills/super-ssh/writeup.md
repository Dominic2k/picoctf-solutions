# 🧩 Challenge: Super SSH

**Category**: General Skills  
**Difficulty**: Easy  
**Event**: picoCTF 2024  
**Tags**: `ssh`, `shell`, `webshell`

---

## 📝 Description

> Using a Secure Shell (SSH) is going to be pretty important.  
> Can you ssh as `ctf-player` to `titan.picoctf.net` at port `64616` to get the flag?  
> You'll also need the password `1ad5be0d`.

---

## 🧠 Objective

Connect to the remote server using SSH to retrieve a flag. This is a basic exercise in using SSH securely and properly.

---

## 💡 Strategy

1. Use the `ssh` command with the username `ctf-player`, host `titan.picoctf.net`, and the given port.
2. When prompted, enter the provided password.
3. Once logged in, look for the flag using basic Linux commands like `ls`, `cat`, `pwd`, etc.

---

## 💻 Commands Used

```bash
ssh ctf-player@titan.picoctf.net -p 64616
