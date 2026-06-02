## What is this?

![](br0kensh3ll.mp4)

br0kensh3ll is a php file that is used in file upload vulnerabilities that will give basic shell access to the attacker if uploaded to a target machine.
<br>
All you need to do is upload the br0kensh3ll.php file to the target machine and enjoy your shell :)

## Change the password

> [!TIP]
> Its recommended to change the default password to enjoy br0kensh3ll alone ;)

Default password: `DefaultPassword123#`

```sh
php -r 'echo password_hash("YOUR_NEW_PASSWORD", PASSWORD_BCRYPT) . "\n";'
```

And replace the outputted hash inside the br0kensh3ll.php file

## Features

- UI at the top displaying system information
- Tab completions for easier command execution
- Warning system for when the target limits PHP command execution
- `upload` command to upload files to the target
- `download` command to download files from the target
- `clear` command to clear the terminal
- `cd` command to navigate the targets system
- `exit` command to terminate the shell

## Limitations

Only linux support
