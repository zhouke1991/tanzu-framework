## tanzu builder completion zsh

Generate the autocompletion script for zsh

### Synopsis

Generate the autocompletion script for the zsh shell.

If shell completion is not already enabled in your environment you will need
to enable it.  You can execute the following once:

	echo "autoload -U compinit; compinit" >> ~/.zshrc

To load completions in your current shell session:

	source <(builder completion zsh); compdef _builder builder

To load completions for every new session, execute once:

#### Linux:

	builder completion zsh > "${fpath[1]}/_builder"

#### macOS:

	builder completion zsh > $(brew --prefix)/share/zsh/site-functions/_builder

You will need to start a new shell for this setup to take effect.


```
tanzu builder completion zsh [flags]
```

### Options

```
  -h, --help              help for zsh
      --no-descriptions   disable completion descriptions
```

### SEE ALSO

* [tanzu builder completion](tanzu_builder_completion.md)	 - Generate the autocompletion script for the specified shell

###### Auto generated by spf13/cobra on 14-Sep-2022
