some method for generate hash and encrypt files

## Encrypt Text
### Encrypt
```
string text = CryptographyHelper.EncryptTextAES("Mahdi", "password");
```
### Decrypt
```
string text = CryptographyHelper.DecryptTextAES("G7Jlxs4gb98msDUOIdN1iA==", "password");
```

***

## Encrypt Files
### Encrypt
```
CryptographyHelper.EncryptFileAES(sourcefile, destination, "password");
```
### Decrypt
```
CryptographyHelper.DecryptFileAES(sourcefile, destination, "password");
```

***
## Generating Hash
### MD5
```
string text = CryptographyHelper.GenerateMD5("mahdi");
// result = F9C24B8F961D48841A9838CCA5274D8D
```

### SHA256
```
string text = CryptographyHelper.GenerateSHA256("mahdi");
// result = 2e0af263c88c69ecc23a51a76b7a2442ed6a9dff080f275a27ec486d1a0e0148
```