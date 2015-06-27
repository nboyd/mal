#####################

# SOURCES_BASE = src/types.rs src/readline.rs \
# 	       src/reader.rs src/printer.rs \
# 	       src/env.rs src/core.rs
# SOURCES_LISP = src/env.rs src/core.rs src/bin/stepA_mal.rs
# SOURCES = $(SOURCES_BASE) $(SOURCES_LISP)

#####################

SRCS = src/step0_repl.rs
BINS = $(SRCS:%.rs=target/release/%)

#####################

all:
	rustc ${SRCS}
# all: mal

# mal: ${SOURCES_BASE} $(word $(words ${SOURCES_LISP}),${SOURCES_LISP})
# 	cargo build --release
# 	cp $(word $(words ${BINS}),${BINS})  $@
#
# #$(BINS): target/release/%: src/%.rs
# #	cargo build --release $*
#
# clean:
# 	cargo clean
# 	rm -f mal
#
# .PHONY: stats stats-lisp mal
#
# stats: $(SOURCES)
# 	@wc $^
# stats-lisp: $(SOURCES_LISP)
# 	@wc $^
