project(files)

install(FILES Library/Documentation/Acknowledgements.rtf DESTINATION libexec/darling/Library/Documentation)
install(FILES
	usr/share/dict/connectives
	usr/share/dict/freebsd
	usr/share/dict/propernames
	usr/share/dict/README
	usr/share/dict/web2
	usr/share/dict/web2a
	DESTINATION
	libexec/darling/usr/share/dict
)

install(FILES
	usr/share/man/man7/intro.7
	usr/share/man/man7/hier.7
	usr/share/man/man7/ascii.7
	usr/share/man/man7/operator.7
	usr/share/man/man7/mailaddr.7
	usr/share/man/man7/hostname.7
	DESTINATION libexec/darling/usr/share/man/man7
)
install(FILES
	usr/share/man/man5/passwd.5
	usr/share/man/man5/hosts.5
	usr/share/man/man5/master.passwd.5
	usr/share/man/man5/services.5
	usr/share/man/man5/motd.5
	usr/share/man/man5/rpc.5
	usr/share/man/man5/networks.5
	usr/share/man/man5/shells.5
	usr/share/man/man5/group.5
	usr/share/man/man5/protocols.5
	usr/share/man/man5/intro.5
	DESTINATION libexec/darling/usr/share/man/man5
)
install(FILES usr/share/man/man8/intro.8 DESTINATION libexec/darling/usr/share/man/man8)

install(FILES
	usr/share/misc/ascii
	usr/share/misc/birthtoken
	usr/share/misc/eqnchar
	usr/share/misc/flowers
	usr/share/misc/getopt
	usr/share/misc/man.template
	usr/share/misc/mdoc.template
	usr/share/misc/operator
	DESTINATION
	libexec/darling/usr/share/misc
)

install(FILES usr/share/sandbox/bsd.sb DESTINATION libexec/darling/usr/share/sandbox)

install(FILES
	private/etc/rpc
	private/etc/update-services.pl
	private/etc/hosts
	private/etc/paths
	private/etc/services
	private/etc/manpaths
	private/etc/protocols
	private/etc/afpovertcp.cfg
	private/etc/networks
	private/etc/gettytab
	private/etc/ftpusers
	private/etc/shells
	private/etc/kern_loader.conf
	private/etc/ttys
	DESTINATION
	libexec/darling/private/etc
)

install(FILES
	private/etc/asl/com.apple.eventmonitor
	private/etc/asl/com.apple.MessageTracer
	private/etc/asl/com.apple.install
	private/etc/asl/com.apple.login.guest
	private/etc/asl/com.apple.mail
	private/etc/asl/com.apple.performance
	DESTINATION
	libexec/darling/private/etc/asl
)

install(FILES private/etc/newsyslog.d/files.conf DESTINATION libexec/darling/private/etc/newsyslog.d)

	
