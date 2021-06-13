# Replit CLI
Welcome to Replit CLI! With the Replit CLI Application, you can work with your repls locally, including clone, pull, and push, the core features of the CLI. The full list of features includes-

```
PS C:\> replit
Usage: replit [OPTIONS] COMMAND [ARGS]...

Options:
  --install-completion [bash|zsh|fish|powershell|pwsh]
								  Install completion for the specified shell.
  --show-completion [bash|zsh|fish|powershell|pwsh]
								  Show completion for the specified shell, to
								  copy it or customize the installation.

  --help                          Show this message and exit.

Commands:
  clone    Clone a Repl's contents to your local machine
  db       Edit the Replit DB for a Repl
  env      Interact with the Environment of the Repl of the Current Working...
  exec     Execute a command to run on the remote repl.
  login    Authenticate with Replit CLI.
  pull     Pull the remote contents of the repl inside the working...
  push     Push changes to the server and override remote.
  run      Run, Stop, or Restart a Repl from your local machine.
  shell    Connect to a bash shell with a remote repl.
  user     Lookup the details for a Replit User
  version  Output the current version for Replit CLI
PS C:\>
```

## Getting an Authentication Token
To start using the core features of Replit CLI however, you will need to authenticate with the CLI Application with your Replit Session ID. Your session ID is a unique identifier linked with your account that acts as a token to access all APIs and Services. To get your sid, look for the cookie that is named ` connect.sid ` when visiting Replit.

To do so, first open the Developer Tools for your browser and open the ` Network ` tab. To open the Developer Tools -

For Safari, you may need to enable the developer menu. See [here](https://support.apple.com/guide/safari/use-the-developer-tools-in-the-develop-menu-sfri20948/mac) for more information.

Once you are sure that your Developer Tools are enabled, (they are enabled by default on Firefox, Chrome, and Edge), use the hotkey ` CTRL + SHIFT + I ` for Windows platforms, and ` CMD + SHIFT + I ` for macOS platforms. This should open a Developer's pane.

![image](https://sjcdn.is-a.dev/file/gqoxgv)

Once you see this pane, click the ` Network ` tab. If necessary, perform a Reload to see HTTP requests. Once HTTP Requests are being shown, search for ` ~ `

![image](https://sjcdn.is-a.dev/file/coojip)

- Click on the request that is requesting the file `~`
- Once clicked, a new pane should pop up
![image](https://sjcdn.is-a.dev/file/qrpxmu)
On this new pane, click the ` Cookies ` tab and copy the value for the cookie named ` connect.sid `. This is your SID token. **DO NOT SHARE THIS WITH ANYONE!** Doing so will grant anyone complete access to your Replit account.

## Logging In
Now that you have your SID value, run the following command -

```
replit login insert_sid_here
```

## Documentation
And you should see a command letting you know that your SID has been saved! Now you are ready to fully use Replit CLI! To see the docs, click [here](https://github.com/CoolCoderSJ/Replit-CLI/wiki)
