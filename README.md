# 🦉 OFtpdX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-ONetwork-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OFtpdX** — FTP Server Configuration Hardening Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OFtpdX — FTP Server Configuration Hardening Auditor. It provides vsftpd — vsftpd.conf, vsftpd.user_list, ftpusers, per-user user_config_dir overrides, anon root, chroot / allow_writeable_chroot, FTPS enforcement, SSLv3 / TLSv1 / ciphers, PORT / PASV promiscuous. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- vsftpd — vsftpd.conf, vsftpd.user_list, ftpusers, per-user user_config_dir overrides, anon root, chroot / allow_writeable_chroot, FTPS enforcement, SSLv3 / TLSv1 / ciphers, PORT / PASV promiscuous
- ProFTPD — Include-aware parser (conf.d, tls.conf, sql.conf, modules.conf), <Anonymous> / <Limit> semantics, mod_copy, DefaultRoot, RootLogin, TLS*, SQL / LDAP credentials, mod_sftp algorithms
- Pure-FTPd — /etc/pure-ftpd/conf one-file-per-option and pure-ftpd.conf, TLS level, anon upload / mkdir, pureftpd.passwd permissions (hashes never read out)
- Cert / key permissions, dpkg version EOL, SFTP hint
- Secrets masked everywhere; --root discovery; CWE + MITRE
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OFtpdX                                     # interactive menu
./OFtpdX --scan -r /path/to/root
./OFtpdX --demo
./OFtpdX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
