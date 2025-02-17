## tanzu kubernetes-release completion zsh

Generate the autocompletion script for zsh

### Synopsis

Generate the autocompletion script for the zsh shell.

If shell completion is not already enabled in your environment you will need
to enable it.  You can execute the following once:

	echo "autoload -U compinit; compinit" >> ~/.zshrc

To load completions in your current shell session:

	source <(kubernetes-release completion zsh); compdef _kubernetes-release kubernetes-release

To load completions for every new session, execute once:

#### Linux:

	kubernetes-release completion zsh > "${fpath[1]}/_kubernetes-release"

#### macOS:

	kubernetes-release completion zsh > $(brew --prefix)/share/zsh/site-functions/_kubernetes-release

You will need to start a new shell for this setup to take effect.


```
tanzu kubernetes-release completion zsh [flags]
```

### Options

```
  -h, --help              help for zsh
      --no-descriptions   disable completion descriptions
```

### Options inherited from parent commands

```
      --log-file string   Log file path
  -v, --verbose int32     Number for the log level verbosity(0-9)
```

### SEE ALSO

* [tanzu kubernetes-release completion](tanzu_kubernetes-release_completion.md)	 - Generate the autocompletion script for the specified shell

###### Auto generated by spf13/cobra on 14-Sep-2022
