Use hg@evgnomon.org

```
Signature key ....: 364A 3C63 EECA E167 CE8F  CF82 66D6 0E50 4F06 A426
      created ....: 2024-04-19 22:34:27
Encryption key....: 8E80 76ED B64E 9F9F 1A89  0609 E6EA ECFB 9A42 C2C7
      created ....: 2024-04-19 22:33:07
```

Apt repo:

```
curl https://evgnomon.org/evgnomon.asc -o - | sudo tee /etc/apt/trusted.gpg.d/evgnomon.asc > /dev/null
sudo tee /etc/apt/sources.list.d/evgnomon.sources << EOF
Types: deb
URIs: https://archive.evgnomon.org/$(. /etc/os-release && echo "$ID")
Suites: $(. /etc/os-release && echo "$VERSION_CODENAME")
Components: main
Signed-By: /etc/apt/trusted.gpg.d/evgnomon.asc
EOF
```

More info: https://evgnomon.org/
