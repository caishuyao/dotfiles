clean:
	@rm -f init.elc config.el config.elc

compile: init.el config.org clean
	@echo "generate config file"
	@emacs -Q --batch -l 'compile.el'

install:
	@echo "install file to emacs dir"
	@cd .. && stow -t ~/emacsdir/csyemacs/ emacs
