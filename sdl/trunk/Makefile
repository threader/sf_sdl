# Makefile for gcc version of SDL

DEFINES= DEFINE=ENABLE_CYBERGRAPHICS DEFINE=inline=__inline DEFINE=ENABLE_AHI DEFINE=NO_SIGNAL_H
# DEFINE=HAVE_OPENGL
#INCLUDES= IDIR=../include
CFLAGS = VERBOSE CPU=68040  CODE=FAR DATA=FAR
#DEBUG=FULL
GCCFLAGS = -I/usr/local/amiga/m68k-amigaos/sys-include/sdl/ -O3 -fomit-frame-pointer -m68040 -mnobitfield \
-DNO_AMIGADEBUG
GLFLAGS = -DSHARED_LIB -DNO_AMIGADEBUG -lamiga

#-I. -I../include -noixemul
GCCDEFINES = -DENABLE_CYBERGRAPHICS -DENABLE_AHI -DNO_SIGNAL_H -D__MEM_AMIGA


GOBJS =  SDL_error.go SDL_fatal.go video/SDL_RLEaccel.go video/SDL_blit.go video/SDL_blit_0.go \
   video/SDL_blit_1.go video/SDL_blit_A.go video/SDL_blit_N.go \
   video/SDL_bmp.go video/SDL_cursor.go video/SDL_pixels.go video/SDL_surface.go video/SDL_stretch.go \
   video/SDL_yuv.go video/SDL_yuv_sw.go video/SDL_video.go audio/SDL_audio.go \
   audio/SDL_audiocvt.go audio/SDL_mixer.go audio/SDL_wave.go audio/amigaos/SDL_ahiaudio.go \
   timer/amigaos/SDL_systimer.go timer/SDL_timer.go joystick/SDL_joystick.go \
   joystick/SDL_sysjoystick.go SDL_cdrom.go SDL_syscdrom.go events/SDL_quit.go events/SDL_active.go \
   events/SDL_keyboard.go events/SDL_mouse.go events/SDL_resize.go file/SDL_rwops.go SDL.go \
   events/SDL_events.go thread/amigaos/SDL_sysmutex.go thread/amigaos/SDL_syssem.go thread/amigaos/SDL_systhread.go thread/amigaos/SDL_thread.go \
   thread/amigaos/SDL_syscond.go video/amigaos/SDL_cgxvideo.go video/amigaos/SDL_cgxmodes.go video/amigaos/SDL_cgximage.go video/amigaos/SDL_amigaevents.go \
   video/amigaos/SDL_amigamouse.go video/amigaos/SDL_cgxgl.go video/amigaos/SDL_cgxwm.go \
   video/amigaos/SDL_cgxyuv.go video/amigaos/SDL_cgxaccel.go video/amigaos/SDL_cgxgl_wrapper.go \
   video/SDL_gamma.go SDL_lutstub.ll stdlib/SDL_stdlib.go stdlib/SDL_string.go stdlib/SDL_malloc.go stdlib/SDL_getenv.go

LOBJS =  SDL_error.lo SDL_fatal.lo video/SDL_RLEaccel.lo video/SDL_blit.lo video/SDL_blit_0.lo \
   video/SDL_blit_1.lo video/SDL_blit_A.lo video/SDL_blit_N.lo \
   video/SDL_bmp.lo video/SDL_cursor.lo video/SDL_pixels.lo video/SDL_surface.lo video/SDL_stretch.lo \
   video/SDL_yuv.lo video/SDL_yuv_sw.lo video/SDL_video.lo audio/SDL_audio.lo \
   audio/SDL_audiocvt.lo audio/SDL_mixer.lo audio/SDL_wave.lo audio/amigaos/SDL_ahiaudio.lo \
   timer/amigaos/SDL_systimer.lo timer/SDL_timer.lo joystick/SDL_joystick.lo \
   joystick/SDL_sysjoystick.lo SDL_cdrom.lo SDL_syscdrom.lo events/SDL_quit.lo events/SDL_active.lo \
   events/SDL_keyboard.lo events/SDL_mouse.lo events/SDL_resize.lo file/SDL_rwops.lo SDL.lo \
   events/SDL_events.lo thread/amigaos/SDL_sysmutex.lo thread/amigaos/SDL_syssem.lo thread/amigaos/SDL_systhread.lo thread/amigaos/SDL_thread.lo \
   thread/amigaos/SDL_syscond.lo video/amigaos/SDL_cgxvideo.lo video/amigaos/SDL_cgxmodes.lo video/amigaos/SDL_cgximage.lo video/amigaos/SDL_amigaevents.lo \
   video/amigaos/SDL_amigamouse.lo video/amigaos/SDL_cgxgl.lo video/amigaos/SDL_cgxwm.lo video/amigaos/SDL_cgxyuv.lo \
   video/amigaos/SDL_cgxaccel.lo video/amigaos/SDL_cgxgl_wrapper.lo \
   video/SDL_gamma.lo SDL_amigastub.lo SDL_lutstubrel.ll stdlib/SDL_stdlib.lo stdlib/SDL_string.lo stdlib/SDL_malloc.lo stdlib/SDL_getenv.lo

MOBJS =  SDL_error.mo SDL_fatal.mo SDL_RLEaccel.mo SDL_blit.mo SDL_blit_0.mo \
   SDL_blit_1.mo SDL_blit_A.mo SDL_blit_N.mo \
   SDL_bmp.mo SDL_cursor.mo SDL_pixels.mo SDL_surface.mo SDL_stretch.mo \
   SDL_yuv.mo SDL_yuv_sw.mo SDL_yuv_mmx.mo SDL_video.mo SDL_audio.mo \
   SDL_audiocvt.mo SDL_audiomem.mo SDL_mixer.mo SDL_wave.mo SDL_ahiaudio.mo \
   SDL_systimer.mo SDL_timer.mo SDL_joystick.mo \
   SDL_sysjoystick.mo SDL_cdrom.mo SDL_syscdrom.mo SDL_quit.mo SDL_active.mo \
   SDL_keyboard.mo SDL_mouse.mo SDL_resize.mo SDL_rwops.mo SDL_endian.mo SDL.mo \
   SDL_events.mo SDL_sysmutex.mo SDL_syssem.mo SDL_systhread.mo SDL_thread.mo \
   SDL_syscond.mo SDL_cgxvideo.mo SDL_cgxmodes.mo SDL_cgximage.mo SDL_amigaevents.mo \
   SDL_amigamouse.mo SDL_cgxgl.mo SDL_cgxwm.mo SDL_cgxyuv.mo SDL_cgxaccel.mo SDL_cgxgl_wrapper.mo \
   SDL_gamma.mo


OBJS = SDL_error.o SDL_fatal.o video/SDL_RLEaccel.o SDL_blit.o SDL_blit_0.o  \
   SDL_blit_1.o SDL_blit_A.o SDL_blit_N.o \
   SDL_bmp.o SDL_cursor.o video/SDL_pixels.o SDL_surface.o SDL_stretch.o \
   SDL_yuv.o SDL_yuv_sw.o SDL_yuv_mmx.o SDL_video.o SDL_audio.o \
   SDL_audiocvt.o SDL_audiomem.o SDL_mixer.o SDL_wave.o SDL_ahiaudio.o \
   SDL_systimer.o SDL_timer.o SDL_joystick.o \
   SDL_sysjoystick.o SDL_cdrom.o SDL_syscdrom.o SDL_quit.o SDL_active.o \
   SDL_keyboard.o SDL_mouse.o SDL_resize.o SDL_rwops.o SDL_endian.o SDL.o \
   SDL_events.o SDL_sysmutex.o SDL_syssem.o SDL_systhread.o SDL_thread.o \
   SDL_syscond.o SDL_cgxvideo.o SDL_cgxmodes.o SDL_cgximage.o SDL_amigaevents.o \
   SDL_amigamouse.o SDL_cgxgl.o SDL_cgxwm.o SDL_cgxyuv.o SDL_cgxaccel.o SDL_cgxgl_wrapper.o \
   SDL_gamma.o stdlib/SDL_stdlib.o

WOBJS =  SDL_error.wo SDL_fatal.wo video/SDL_RLEaccel.wo SDL_blit.wo SDL_blit_0.wo \
   SDL_blit_1.wo SDL_blit_A.wo SDL_blit_N.wo \
   SDL_bmp.wo SDL_cursor.wo SDL_pixels.wo SDL_surface.wo SDL_stretch.wo \
   SDL_yuv.wo SDL_yuv_sw.wo SDL_yuv_mmx.wo SDL_video.wo SDL_audio.wo \
   SDL_audiocvt.wo SDL_audiomem.wo SDL_mixer.wo SDL_wave.wo SDL_ahiaudio.wo \
   SDL_systimer.wo SDL_timer.wo SDL_joystick.wo \
   SDL_sysjoystick.wo SDL_cdrom.wo SDL_syscdrom.wo SDL_quit.wo SDL_active.wo \
   SDL_keyboard.wo SDL_mouse.wo SDL_resize.wo SDL_rwops.wo SDL_endian.wo SDL.wo \
   SDL_events.wo SDL_sysmutex.wo SDL_syssem.wo SDL_systhread.wo SDL_thread.wo \
   SDL_syscond.wo SDL_cgxvideo.wo SDL_cgxmodes.wo SDL_cgximage.wo SDL_amigaevents.wo \
   SDL_amigamouse.wo SDL_cgxgl.wo SDL_cgxwm.wo SDL_cgxyuv.wo SDL_cgxaccel.wo SDL_cgxgl_wrapper.wo \
   SDL_gamma.wo stdlib/SDL_stdlib.wo
   
%.go: %.c
	$(CC) $(GCCFLAGS) $(GCCDEFINES) -o $@ -c $*.c

#%.lo: %.c
#	$(CC) $(GCCFLAGS) $(GLFLAGS) $(INCLUDES) $(GCCDEFINES) -o $@ -c $*.c

#%.so: %.c
#	sc $(CFLAGS) $(DEFINES) LIBCODE NOSTACKCHECK $(INCLUDES) OBJNAME $@  $*.c

%.ll: %.s
	$(AS) -m68040 -o $@ $*.s

#%.mo: %.c
#	ppc-morphos-gcc $(GCCFLAGS) $(GCCDEFINES) -Isf0:ggmorphos/os-include/ -DMORPHOS -o $@ -c $*.c

%.o: %.c
	SC $(CFLAGS) $(DEFINES) $(INCLUDES) $*.c

#%.wo: %.c
#	ppc-amigaos-gcc -warpup $(GCCFLAGS) $(GCCDEFINES) -DWARPOS -DNO_AMIGADEBUG -o $@ -c $*.c

all: libSDL.a SDL.library  libSDLstub.a libSDL_mos.a SDL.lib 

libSDLstub.a: SDLstub.go
	ar cru libSDLstub.a SDLstub.go
	/usr/local/amiga/bin/ranlib libSDLstub.a

SDL.lib: $(OBJS)
	-rm -f sdl.lib
	sc OBJLIB=SDL.lib $(OBJS) NODEBUG

SDL.library: $(LOBJS)
	$(CC) -v -s -resident -nostdlib -lamiga /usr/local/m68k-amigaos/lib/libnix/libinitr.o $(LOBJS) \
     /usr/local/m68k-amigaos/lib/libgcc.a /usr/local/m68k-amigaos/lib/libb/libnix/libnix.a  \
     /usr/local/m68k-amigaos/lib/libb/libnix/libm.a  -o $@ -ldebug

# gg:lib/libb/libnix/libnix.a gg:lib/libb/libnix/libstubs.a  gg:lib/libb/libnix/libm.a -o $@ -ldebug

#	slink to $@ LIBFD SDL.fd lib lib:sc.lib lib:scm.lib lib:debug.lib noicons libversion 1 librevision 2 smalldata stripdebug libprefix _LIB from lib:libent.o lib:libinitr.o $(OBJS) SDL_amigasas.so
#	gcc -v -fbaserel -nostartfiles -noixemul gg:lib/libnix/libinitr.o $(LOBJS) -o $@ -lm -ldebug
#	gcc -v -s -resident -nostdlib gg:lib/libnix/libinitr.o $(LOBJS) -o $@ -ldebug

libSDL.a: $(GOBJS)
	-rm -f libSDL.a
	ar cru libSDL.a $(GOBJS)
	/usr/local/amiga/bin/ranlib libSDL.a
	-cp libSDL.a /usr/local/amiga/m68k-amigaos/lib

libSDL_mos.a: $(MOBJS)
	-rm -f libSDL_mos.a
	ppc-morphos-ar cru libSDL_mos.a $(MOBJS)
	ppc-morphos-ranlib libSDL_mos.a

libSDL_wos.a: $(WOBJS)
	-rm -f lib/libSDL_wos.a
	ppc-amigaos-ar cru libSDL_wos.a $(WOBJS)
	ppc-amigaos-ranlib libSDL_wos.a
 
clean: 
	-rm -f $(LOBJS) 
	-rm -f $(GOBJS)
	-rm -f $(MOBJS)
   


