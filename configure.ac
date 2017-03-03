#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT( ape , [1.0] )
AM_INIT_AUTOMAKE

AC_CONFIG_FILES([Makefile
                 src/Makefile
                 include/Makefile])

AC_CONFIG_SRCDIR([src/pil_error.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC

# Checks for libraries.
AC_SEARCH_LIBS(free_readline_memory ,
               readline ,
               [use_readline=yes])

# Checks for header files.
AC_CHECK_HEADERS([float.h limits.h malloc.h stddef.h stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_STRTOD
AC_CHECK_FUNCS([atexit gethostname memchr memset setenv strchr strrchr strstr strtol])

AC_OUTPUT