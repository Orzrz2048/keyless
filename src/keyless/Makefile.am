ACLOCAL_AMFLAGS = -I m4

bin_PROGRAMS=keyless testclient
noinst_LTLIBRARIES=libkeyless_common.la

# 构建 keyless 服务和 testclient 依赖的公共组件
libkeyless_common_la_SOURCES=kssl_helpers.c kssl_log.c

# 构建 keyless 服务
keyless_SOURCES=keyless.c kssl_core.c kssl_private_key.c kssl_thread.c kssl_getopt.c
keyless_LDADD= -lcrypto -lssl -ldl -lpthread -lrt -luv libkssl_helpers.la
#keyless_LDFLAGS='-Wl,-rpath,/usr/local/lib'

# 构建 testclient
testclient_SOURCES=testclient.c 
testclient_LDADD= -lcrypto -lssl -ldl -lpthread -lrt -luv libkssl_helpers.la
#testclient_LDFLAGS='-Wl,-rpath,/usr/local/lib'