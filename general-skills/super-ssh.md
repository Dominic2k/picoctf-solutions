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

## 🎯 Objective

Kết nối SSH để truy cập máy chủ từ xa và tìm flag.

---

## 🧠 Strategy

1. Dùng lệnh `ssh` để kết nối với server.
2. Nhập mật khẩu.
3. Dùng các lệnh cơ bản trong shell như `ls`, `cat`, `cd`, v.v.
4. Tìm và đọc file chứa flag.

---

## 💻 Commands & Execution Log

```bash
$ ssh ctf-player@titan.picoctf.net -p 64616
Password: 1ad5be0d

$ ls
flag.txt

$ cat flag.txt
picoCTF{5sh_i5_5uP3r_Us3fu1!}
