## r12.06.26-2
	* GsDoc now supports local, package-global and imported package variables and functions
		(MarGo/doc is still incomplete, however: types(structs, etc.) are not resolved yet)
		I've changed the way GsDoc works. Both mode are unified, ctrl+dot,ctrl+g will take you to
		the definition but the hint( ctrl+dot,ctrl+h ) now displays the src along with any comments
		attached to it (this is usually pure documentation)
	* MarGo needs updating

## r12.06.26-1
	* fix: file saving in gsshell
	* fix: duplicating comment that follows imports when imports are modified
	* fix: adding duplicate entries to the package list due to filename case-insensitivity
	* the new_go_file command now automatically fills out the package declaration
	* add binding to create a new go file ( ctrl+dot,ctrl+n )

## r12.06.17-1
	* add support for running(play) the current file without saving it (`ctrl+dot`, `ctrl+r`)
	* add support for sharing the contents of the current on play.golang.org
	press `ctrl+dot`, `ctrl+dot` for a list of all commands and their key bindings as well sharing functionality

## r12.06.09-2
	* MarGo now supports warning about calling flag.String() etc and forgetting to call flag.Parse() afterwards

## r12.06.09-1
	* removed ctrl+shift+g keybinding, please use `ctrl+dot`,`ctrl+dot` to show the list of available commands and their kebindings
	* complete implementation of imports:
	      use `ctrl+dot`,`ctrl+p` to add or remove packages
	      use `ctrl+dot`,`ctrl+i` to quickly jump to the last imported package where you can assign an alias, etc.
	      use `ctrl+dot`,`ctrl+[` to go back to where you were before
	* MarGo needs updating and a restart of ST2 is recommended

## r12.06.05-1
	* add support for configuring the fmt tab settings - see GoSublime.sublime-settings (fmt_tab_width and fmt_tab_indent)

## r12.06.02-1
	* Add initial stub implementation of goto-definition and show-documentation
	*     this requires the latest version of MarGo
	* new key bindings and commands: press `ctrl+.`, `ctrl+.`
	*     (control or super on OS X, followed by .(dot) twice)
	*     or open the command palette(`ctrl+shift+p`) and type `GoSublime:`
	*     to show a list of available commands and their respective key bindings
	* note: currently only the pkgname.Function is supported, so types, methods or constants, etc.

## r12.05.30-1
	* fix completion only offering the 'import snippet' if there aren't any imports in the file

## r12.05.29-1
	* update MarGo

## r12.05.26-2
	* re-enable linting

## r12.05.26-1
	* start using margo.fmt, no more dependecy on `gofmt` and `diff`

## r12.05.05-1
	* add support for installing/updating Gocode and MarGo
