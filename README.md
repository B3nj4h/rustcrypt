# Rustcrypt
RustCrypt: Because even your files need a good, old-fashioned cloak-and-dagger routine! This Rust tool encrypts and decrypts files like a secret agent with a taste for code-breaking. Your data's new motto? 'Shhh, I'm encrypted!'" 🔒🕵️‍♂️
# Usage
The tool can be used the same way for both encrpting and decrypting of both small and large files
# Arguments

```bash
./rustcrypt --help
        
 ██████╗  ██╗   ██╗  ███████╗ ████████╗  ██████╗  ██████╗  ██╗   ██╗  ██████╗  ████████╗
 ██╔══██╗ ██║   ██║  ██╔════╝ ╚══██╔══╝ ██╔════╝  ██╔══██╗ ╚██╗ ██╔╝  ██╔══██╗ ╚══██╔══╝
 ██████╔╝ ██║   ██║  ███████╗    ██║    ██║       ██████╔╝  ╚████╔╝   ██████╔╝    ██║   
 ██╔══██╗ ██║   ██║  ╚════██║    ██║    ██║       ██╔══██╗   ╚██╔╝    ██╔═══╝     ██║   
 ██║  ██║ ╚██████╔╝  ███████║    ██║    ╚██████╗  ██║  ██║    ██║     ██║         ██║   
 ╚═╝  ╚═╝  ╚═════╝   ╚══════╝    ╚═╝     ╚═════╝  ╚═╝  ╚═╝    ╚═╝     ╚═╝         ╚═╝   

 Myst3ry
 Version: 1.0.0 
 Usage: rustcrypt [OPTIONS] --input <INPUT> --output <OUTPUT> --size <SIZE> --mode <MODE> 
 Options:
  -i, --input <INPUT>    Input file path
  -o, --output <OUTPUT>  Output file path with key
  -s, --size <SIZE>      file size = [large, small]
  -m, --mode <MODE>      type of mode = [encrypt, decrypt]
  -k, --key <KEY>        Key to decrypt file
  -n, --nonce <NONCE>    nonce to decrypt file
  -h, --help             Print help
  -V, --version          Print version
```
# Encrypt a file

```bash
./rustcrypt -i ~/Documents/test/notes -o ~/Documents/test/enc --size small --mode encrypt
        
 ██████╗  ██╗   ██╗  ███████╗ ████████╗  ██████╗  ██████╗  ██╗   ██╗  ██████╗  ████████╗
 ██╔══██╗ ██║   ██║  ██╔════╝ ╚══██╔══╝ ██╔════╝  ██╔══██╗ ╚██╗ ██╔╝  ██╔══██╗ ╚══██╔══╝
 ██████╔╝ ██║   ██║  ███████╗    ██║    ██║       ██████╔╝  ╚████╔╝   ██████╔╝    ██║   
 ██╔══██╗ ██║   ██║  ╚════██║    ██║    ██║       ██╔══██╗   ╚██╔╝    ██╔═══╝     ██║   
 ██║  ██║ ╚██████╔╝  ███████║    ██║    ╚██████╗  ██║  ██║    ██║     ██║         ██║   
 ╚═╝  ╚═╝  ╚═════╝   ╚══════╝    ╚═╝     ╚═════╝  ╚═╝  ╚═╝    ╚═╝     ╚═╝         ╚═╝   

3ncrypt3d succ3ssfully
Save the key and the nonce safely
----------------------------------------------------------

{

  Key :"iFwHx2uLQ37uOwrobSQT6IXS3icURvxAyJfIKT3sKMA"

  Nonce :"DlNlQoKttjX7EAdWBg4Sxp14duP381/w"

}

----------------------------------------------------------
```

# Decrypt a file

```bash
./rustcrypt -i ~/Documents/test/enc -o ~/Documents/test/dec --size small --mode decrypt -k 55iN8J5Nywxh4m0tYUoYSC5GVYrn0MoUs+02qsSGk/g -n aTCrxrZEp4l4/f6gs5JunE83MXt5ZyQi
        
 ██████╗  ██╗   ██╗  ███████╗ ████████╗  ██████╗  ██████╗  ██╗   ██╗  ██████╗  ████████╗
 ██╔══██╗ ██║   ██║  ██╔════╝ ╚══██╔══╝ ██╔════╝  ██╔══██╗ ╚██╗ ██╔╝  ██╔══██╗ ╚══██╔══╝
 ██████╔╝ ██║   ██║  ███████╗    ██║    ██║       ██████╔╝  ╚████╔╝   ██████╔╝    ██║   
 ██╔══██╗ ██║   ██║  ╚════██║    ██║    ██║       ██╔══██╗   ╚██╔╝    ██╔═══╝     ██║   
 ██║  ██║ ╚██████╔╝  ███████║    ██║    ╚██████╗  ██║  ██║    ██║     ██║         ██║   
 ╚═╝  ╚═╝  ╚═════╝   ╚══════╝    ╚═╝     ╚═════╝  ╚═╝  ╚═╝    ╚═╝     ╚═╝         ╚═╝   

D3crpt3d succ3ssfully
```
