plugin_LTLIBRARIES = libgstdirectsoundsrc.la

libgstdirectsoundsrc_la_SOURCES = gstdirectsoundsrc.c gstdirectsoundplugin.c
libgstdirectsoundsrc_la_CFLAGS = $(GST_CFLAGS) $(GST_BASE_CFLAGS) \
	$(GST_PLUGINS_BASE_CFLAGS) $(DIRECTX_CFLAGS)
libgstdirectsoundsrc_la_LIBADD = \
	$(GST_BASE_LIBS) $(GST_PLUGINS_BASE_LIBS) -lgstaudio-$(GST_API_VERSION) \
	$(DIRECTX_LDFLAGS) $(DIRECTSOUND_LIBS) -lole32
libgstdirectsoundsrc_la_LDFLAGS = $(GST_PLUGIN_LDFLAGS)

noinst_HEADERS= gstdirectsoundsrc.h
