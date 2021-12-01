AC_PREREQ([2.68])
# 设置包名称 dtcs-engine，版本号 1.0
AC_INIT([keyless-engine], [1.0], [])
AC_CONFIG_SRCDIR([src/engine/e_keyless.c])
AC_CONFIG_SRCDIR([src/server/keyless.c])
AC_CONFIG_SRCDIR([src/lib/kssl_core.c])
# 设置 automake 的选项列表
# -Wall 和 -Werror 要求 automake 打开所有警告并将它们报告为错误
#  foreign 表明这个包不会遵循 GNU 标准
AM_INIT_AUTOMAKE([foreign subdir-objects])

AC_CONFIG_MACRO_DIR([m4])
# 该文件中定义的宏将保存在 config.h 文件中
AC_CONFIG_HEADERS([config.h])

#Libtool for generating shared library
LT_INIT
AC_PROG_LN_S
AC_CONFIG_MACRO_DIR([m4])

AC_PROG_CC
AC_PROG_CC_STDC
AC_PROG_LIBTOOL
AM_PROG_LIBTOOL

AC_CHECK_HEADERS([openssl/engine.h])

AC_CONFIG_FILES([
	Makefile
	src/Makefile])
AC_OUTPUT