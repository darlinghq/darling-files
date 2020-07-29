project(files)

install(
	DIRECTORY Library
	DESTINATION libexec/darling
	PATTERN "Makefile" EXCLUDE
)
install(
	DIRECTORY private
	DESTINATION libexec/darling
	PATTERN "Makefile" EXCLUDE
	PATTERN "*.iPhone" EXCLUDE
)
install(
	DIRECTORY System
	DESTINATION libexec/darling
	PATTERN "Makefile" EXCLUDE
	PATTERN "*.py" EXCLUDE
)
install(
	DIRECTORY usr
	DESTINATION libexec/darling
	PATTERN "Makefile" EXCLUDE
	PATTERN "firmlinks" EXCLUDE
)

# TODO: perform many of the same install actions that Apple's Makefiles are supposed to
# e.g. running the Python scripts in `System/Library/DirectoryServices/DefaultLocalDB` to setup the base `master.passwd` and `group`
