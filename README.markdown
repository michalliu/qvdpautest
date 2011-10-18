# qvdpautest - VDPAU Testing Tool

This is a little VDPAU benchmarking tool.
For example, there are the results on a GT216 :

    qvdpautest 0.5
    Intel(R) Core(TM)2 CPU         E8500  @ 3.16GHz
    NVIDIA GPU GeForce GT 220 (GT216) at PCI:1:0:0 (GPU-0)
    
    VDPAU API version : 1
    VDPAU implementation : NVIDIA VDPAU Driver Shared Library  195.22  Sun Nov 22 17:37:18 PST 2009
 
    SURFACE GET BITS: 1190.48 M/s
    SURFACE PUT BITS: 851.243 M/s
 
    MPEG DECODING (1920x1080): 70 frames/s
    MPEG DECODING (1280x720): 163 frames/s
    H264 DECODING (1920x1080): 66 frames/s
    H264 DECODING (1280x720): 138 frames/s
    VC1 DECODING (1440x1080): 83 frames/s
    MPEG4 DECODING (1920x1080): 72 frames/s
 
    MIXER WEAVE (1920x1080): 1053 frames/s
    MIXER BOB (1920x1080): 1815 fields/s
    MIXER TEMPORAL (1920x1080): 478 fields/s
    MIXER TEMPORAL + IVTC (1920x1080): 313 fields/s
    MIXER TEMPORAL + SKIP_CHROMA (1920x1080): 637 fields/s
    MIXER TEMPORAL_SPATIAL (1920x1080): 176 fields/s
    MIXER TEMPORAL_SPATIAL + IVTC (1920x1080): 145 fields/s
    MIXER TEMPORAL_SPATIAL + SKIP_CHROMA (1920x1080): 194 fields/s
    MIXER TEMPORAL_SPATIAL (720x576 video to 1920x1080 display): 623 fields/s
    MIXER TEMPORAL_SPATIAL + HQSCALING (720x576 video to 1920x1080 display): 293 fields/s
  
    MULTITHREADED MPEG DECODING (1920x1080): 72 frames/s
    MULTITHREADED MIXER TEMPORAL (1920x1080): 370 fields/s

## Required Dependencies

You will require the following dependencies:

 - A basic build environment with C++
 - qt Dev Tools (like qmake)
 - Something that will provide libvdpau.so

This is not an exhaustive list but will highlight some things that you will need.

## Compile and run:

qmake ( or qmake-qt4 )
make

(SET POWERMIZER TO "Maximum Performance")
./qvdpautest

## Questions and Comments 

Lemme know if it doesn't work as expected.
hftom@free.fr

