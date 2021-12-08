ACLOCAL_AMFLAGS = -I m4

lib_LTLIBRARIES=libkeyless.la

# 构建 keyless-engine
libkeyless_la_SOURCES=e_keyless.c keyless_rsa.c
libkeyless_la_LIBADD= -lssl -lcrypto ../keyless/libkeyless_common.la
libkeyless_la_LDFLAGS= -module -shared