basedir = mmx
include $(top_srcdir)/modules/common.am

libi420_rgb_mmx_plugin_la_SOURCES = \
        ../video_chroma/i420_rgb.c \
	../video_chroma/i420_rgb.h \
        ../video_chroma/i420_rgb16.c \
        i420_rgb_mmx.h
libi420_rgb_mmx_plugin_la_CFLAGS = $(AM_CFLAGS)
libi420_rgb_mmx_plugin_la_LIBADD = $(AM_LIBADD)
if HAVE_WIN32
libi420_rgb_mmx_plugin_la_DEPENDENCIES = libi420_rgb_mmx_plugin.rc.o
endif

libi420_yuy2_mmx_plugin_la_SOURCES = \
        ../video_chroma/i420_yuy2.c \
	../video_chroma/i420_yuy2.h
libi420_yuy2_mmx_plugin_la_CFLAGS = $(AM_CFLAGS)
libi420_yuy2_mmx_plugin_la_LIBADD = $(AM_LIBADD)
if HAVE_WIN32
libi420_yuy2_mmx_plugin_la_DEPENDENCIES = libi420_yuy2_mmx_plugin.rc.o
endif

libi422_yuy2_mmx_plugin_la_SOURCES = \
        ../video_chroma/i422_yuy2.c \
	../video_chroma/i422_yuy2.h
libi422_yuy2_mmx_plugin_la_CFLAGS = $(AM_CFLAGS)
libi422_yuy2_mmx_plugin_la_LIBADD = $(AM_LIBADD)
if HAVE_WIN32
libi422_yuy2_mmx_plugin_la_DEPENDENCIES = libi422_yuy2_mmx_plugin.rc.o
endif

libvlc_LTLIBRARIES = \
	libi420_rgb_mmx_plugin.la \
	libi420_yuy2_mmx_plugin.la \
	libi422_yuy2_mmx_plugin.la
