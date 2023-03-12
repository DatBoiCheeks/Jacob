# Jacob
Minecraft Java wont run




#
# A fatal error has been detected by the Java Runtime Environment:
#
#  EXCEPTION_ACCESS_VIOLATION (0xc0000005) at pc=0x00007ffecbe61c42, pid=8180, tid=19352
#
# JRE version: OpenJDK Runtime Environment Microsoft-32931 (17.0.3+7) (build 17.0.3+7-LTS)
# Java VM: OpenJDK 64-Bit Server VM Microsoft-32931 (17.0.3+7-LTS, mixed mode, tiered, compressed oops, compressed class ptrs, g1 gc, windows-amd64)
# Problematic frame:
# C  [atio6axx.dll+0x131c42]
#
# No core dump will be written. Minidumps are not enabled by default on client versions of Windows
#
# If you would like to submit a bug report, please visit:
#   https://github.com/microsoft/openjdk/issues
# The crash happened outside the Java Virtual Machine in native code.
# See problematic frame for where to report the bug.
#

---------------  S U M M A R Y ------------

Command Line: -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Dos.name=Windows 10 -Dos.version=10.0 -Xss1M -Djava.library.path=C:\Users\Jacob\AppData\Roaming\.minecraft\bin\44685878b69bb36a6fb05390c06c8b0243d34f57 -Dminecraft.launcher.brand=minecraft-launcher -Dminecraft.launcher.version=2.3.645 -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M -Dlog4j.configurationFile=C:\Users\Jacob\AppData\Roaming\.minecraft\assets\log_configs\client-1.12.xml net.minecraft.client.main.Main --username DatBoiCheeks --version 1.19.3 --gameDir C:\Users\Jacob\AppData\Roaming\.minecraft --assetsDir C:\Users\Jacob\AppData\Roaming\.minecraft\assets --assetIndex 2 --uuid a8c1aefee98b4677b783dc1beb0b04bc -heuVB5ZQTRgGhrTuT1-YufL5tQ --clientId NWVmYjhkZDktNjEzZi00ZjNmLTlkZDgtMjBjNmNlZWMzNDBl --xuid 2535432210837001 --userType msa --versionType release

Host: AMD Ryzen 7 5800H with Radeon Graphics         , 16 cores, 15G,  Windows 11 , 64 bit Build 22621 (10.0.22621.1344)
Time: Sun Mar 12 15:07:36 2023 Central Daylight Time elapsed time: 7.358334 seconds (0d 0h 0m 7s)

---------------  T H R E A D  ---------------

Current thread (0x000002108454c450):  JavaThread "Render thread" [_thread_in_native, id=19352, stack(0x000000398ee00000,0x000000398ef00000)]

Stack: [0x000000398ee00000,0x000000398ef00000],  sp=0x000000398eefdd00,  free space=1015k
Native frames: (J=compiled Java code, j=interpreted, Vv=VM code, C=native code)
C  [atio6axx.dll+0x131c42]

Java frames: (J=compiled Java code, j=interpreted, Vv=VM code)
j  org.lwjgl.system.JNI.invokePPPP(IIJJJJ)J+0
j  org.lwjgl.glfw.GLFW.nglfwCreateWindow(IIJJJ)J+14
j  org.lwjgl.glfw.GLFW.glfwCreateWindow(IILjava/lang/CharSequence;JJ)J+34
j  edh.<init>(Ledi;Ledf;Lecv;Ljava/lang/String;Ljava/lang/String;)V+281
j  fek.a(Lecv;Ljava/lang/String;Ljava/lang/String;)Ledh;+15
j  ejf.<init>(Leue;)V+761
j  net.minecraft.client.main.Main.a([Ljava/lang/String;Z)V+1348
j  net.minecraft.client.main.Main.main([Ljava/lang/String;)V+2
v  ~StubRoutines::call_stub

siginfo: EXCEPTION_ACCESS_VIOLATION (0xc0000005), writing address 0x0000000000000060


Register to memory mapping:

RIP=0x00007ffecbe61c42 atio6axx.dll
RAX=0x0 is NULL
RBX=0x0 is NULL
RCX=0x00007ffecc84ceb0 atio6axx.dll
RDX=0x0 is NULL
RSP=0x000000398eefdd00 is pointing into the stack for thread: 0x000002108454c450
RBP=0x0000000000000012 is an unknown value
RSI=0x000000398eefdf00 is pointing into the stack for thread: 0x000002108454c450
RDI=0x00007ffecf75c6c0 atio6axx.dll
R8 =0x00000210a13ac080 points into unknown readable memory: 0xf700b63d00b20419 | 19 04 b2 00 3d b6 00 f7
R9 =0x0000000000000001 is an unknown value
R10=0x0000021082290000 points into unknown readable memory: 0x0000000000000000 | 00 00 00 00 00 00 00 00
R11=0x000000398eefdbc0 is pointing into the stack for thread: 0x000002108454c450
R12=0x00007fff2e45bf24 atig6pxx.dll
R13={method} {0x00000210ab0e7b90} 'invokePPPP' '(IIJJJJ)J' in 'org/lwjgl/system/JNI'
R14=0x00007ffee80e54a0 opengl32.dll
R15=0x00007fff2e45c14c atig6pxx.dll


Registers:
RAX=0x0000000000000000, RBX=0x0000000000000000, RCX=0x00007ffecc84ceb0, RDX=0x0000000000000000
RSP=0x000000398eefdd00, RBP=0x0000000000000012, RSI=0x000000398eefdf00, RDI=0x00007ffecf75c6c0
R8 =0x00000210a13ac080, R9 =0x0000000000000001, R10=0x0000021082290000, R11=0x000000398eefdbc0
R12=0x00007fff2e45bf24, R13=0x00000210ab0e7b88, R14=0x00007ffee80e54a0, R15=0x00007fff2e45c14c
RIP=0x00007ffecbe61c42, EFLAGS=0x0000000000010202

Top of Stack: (sp=0x000000398eefdd00)
0x000000398eefdd00:   0000000000000000 0000000000000000
0x000000398eefdd10:   00007ffecf707290 00007fff2e45bf24
0x000000398eefdd20:   00007ffecf75c6c0 000000398eefdf00
0x000000398eefdd30:   0000000000000012 00007ffecdd2389c
0x000000398eefdd40:   0000000000000000 0000000000000028
0x000000398eefdd50:   32353833425c3038 366f6974615c0000
0x000000398eefdd60:   0000000000000028 00007ffecdd5322c
0x000000398eefdd70:   0000000000000000 0000000000000000
0x000000398eefdd80:   0000e23419bb3311 00007fff628e3310
0x000000398eefdd90:   00007ffecf75c6c0 00007ffecbe61a87
0x000000398eefdda0:   0000000000000000 0000000000000012
0x000000398eefddb0:   000000398eefdf00 0000000000000000
0x000000398eefddc0:   00007ffecf75c6b8 00007ffecbe616f5
0x000000398eefddd0:   00007ffecf75c6c0 0000000000000000
0x000000398eefdde0:   00000210a01e9100 000000398eefdf00
0x000000398eefddf0:   0000000000000009 00007ffecbe5b754 

Instructions: (pc=0x00007ffecbe61c42)
0x00007ffecbe61b42:   7d 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 db
0x00007ffecbe61b52:   7a 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 cb
0x00007ffecbe61b62:   78 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 bb
0x00007ffecbe61b72:   76 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 7b
0x00007ffecbe61b82:   72 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 1b
0x00007ffecbe61b92:   6e 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 db
0x00007ffecbe61ba2:   69 00 00 cc cc cc cc cc cc cc cc cc cc cc e9 ef
0x00007ffecbe61bb2:   15 ef 01 cc cc cc cc cc cc cc cc cc cc cc 48 89
0x00007ffecbe61bc2:   5c 24 08 48 89 6c 24 10 48 89 74 24 18 57 48 81
0x00007ffecbe61bd2:   ec 90 00 00 00 48 8b 05 2a a4 71 03 48 33 c4 48
0x00007ffecbe61be2:   89 84 24 80 00 00 00 48 8b 0d 38 a8 89 03 48 8b
0x00007ffecbe61bf2:   01 ff 10 0f 57 c0 0f 11 05 19 b7 8f 03 0f 11 05
0x00007ffecbe61c02:   22 b7 8f 03 0f 11 05 2b b7 8f 03 33 d2 41 b8 88
0x00007ffecbe61c12:   0a 00 00 48 8d 0d 4c ac 8f 03 e8 7f af e6 01 48
0x00007ffecbe61c22:   8d 0d 40 ac 8f 03 e8 c3 4a 34 00 b1 01 e8 2c 87
0x00007ffecbe61c32:   9e 00 48 89 05 dd aa 8f 03 48 8d 0d 6e b2 9e 00
0x00007ffecbe61c42:   48 89 48 60 48 8d 44 24 20 48 89 44 24 58 48 8b
0x00007ffecbe61c52:   05 91 a6 89 03 4c 8b 10 ba 78 00 00 00 33 c9 41
0x00007ffecbe61c62:   b9 01 00 00 80 44 8d 42 90 41 ff 52 08 48 8b f0
0x00007ffecbe61c72:   48 89 44 24 60 48 89 44 24 68 33 ff 48 85 c0 74
0x00007ffecbe61c82:   54 48 89 38 48 89 78 08 48 89 78 10 48 89 78 58
0x00007ffecbe61c92:   48 89 78 60 48 8d 58 68 48 89 5c 24 30 48 89 3b
0x00007ffecbe61ca2:   48 89 7b 08 8d 4f 30 e8 e2 74 e6 01 48 89 00 48
0x00007ffecbe61cb2:   89 40 08 48 89 40 10 66 c7 40 18 01 01 48 89 03
0x00007ffecbe61cc2:   0f 57 c0 0f 11 46 18 0f 11 46 28 0f 11 46 38 0f
0x00007ffecbe61cd2:   11 46 48 eb 03 48 8b f7 48 8b 1d 27 aa 8f 03 48
0x00007ffecbe61ce2:   8b 43 08 48 89 44 24 40 89 7c 24 48 48 8b cb 80
0x00007ffecbe61cf2:   78 19 00 75 22 66 0f 1f 84 00 00 00 00 00 48 89
0x00007ffecbe61d02:   44 24 40 c7 44 24 48 01 00 00 00 48 8b c8 48 8b
0x00007ffecbe61d12:   00 80 78 19 00 74 e7 80 79 19 00 75 06 83 79 20
0x00007ffecbe61d22:   00 76 68 48 b8 55 55 55 55 55 55 55 05 48 39 05
0x00007ffecbe61d32:   da a9 8f 03 0f 84 27 01 00 00 48 8d 2d c5 a9 8f 


Stack slot to memory mapping:
stack at sp + 0 slots: 0x0 is NULL
stack at sp + 1 slots: 0x0 is NULL
stack at sp + 2 slots: 0x00007ffecf707290 atio6axx.dll
stack at sp + 3 slots: 0x00007fff2e45bf24 atig6pxx.dll
stack at sp + 4 slots: 0x00007ffecf75c6c0 atio6axx.dll
stack at sp + 5 slots: 0x000000398eefdf00 is pointing into the stack for thread: 0x000002108454c450
stack at sp + 6 slots: 0x0000000000000012 is an unknown value
stack at sp + 7 slots: 0x00007ffecdd2389c atio6axx.dll


---------------  P R O C E S S  ---------------

Threads class SMR info:
_java_thread_list=0x00000210a8e3c690, length=33, elements={
0x000002108454c450, 0x000002109f0b7df0, 0x000002109f0b87a0, 0x000002109f126430,
0x000002109f126cf0, 0x000002109f127ab0, 0x000002109f128c70, 0x000002109f12cf00,
0x000002109f12d9a0, 0x000002109f12ff90, 0x000002109fd2a3f0, 0x000002109fd58010,
0x000002109fd61d70, 0x000002109fd6a040, 0x00000210a0e614f0, 0x00000210a143da80,
0x00000210a150e910, 0x00000210a150c290, 0x00000210a150cc30, 0x00000210a150d100,
0x00000210a150ede0, 0x00000210a150b8f0, 0x00000210a31e0550, 0x00000210a31e2700,
0x00000210a31dda00, 0x00000210a31dcb90, 0x00000210a31e2bd0, 0x00000210a31e3570,
0x00000210a31ded40, 0x00000210a31df6e0, 0x00000210a31dfbb0, 0x00000210a31e3a40,
0x00000210a31e30a0
}

Java Threads: ( => current thread )
=>0x000002108454c450 JavaThread "Render thread" [_thread_in_native, id=19352, stack(0x000000398ee00000,0x000000398ef00000)]
  0x000002109f0b7df0 JavaThread "Reference Handler" daemon [_thread_blocked, id=12484, stack(0x000000398f500000,0x000000398f600000)]
  0x000002109f0b87a0 JavaThread "Finalizer" daemon [_thread_blocked, id=7148, stack(0x000000398f600000,0x000000398f700000)]
  0x000002109f126430 JavaThread "Signal Dispatcher" daemon [_thread_blocked, id=15712, stack(0x000000398f700000,0x000000398f800000)]
  0x000002109f126cf0 JavaThread "Attach Listener" daemon [_thread_blocked, id=2456, stack(0x000000398f800000,0x000000398f900000)]
  0x000002109f127ab0 JavaThread "Service Thread" daemon [_thread_blocked, id=18680, stack(0x000000398f900000,0x000000398fa00000)]
  0x000002109f128c70 JavaThread "Monitor Deflation Thread" daemon [_thread_blocked, id=12080, stack(0x000000398fa00000,0x000000398fb00000)]
  0x000002109f12cf00 JavaThread "C2 CompilerThread0" daemon [_thread_blocked, id=16444, stack(0x000000398fb00000,0x000000398fc00000)]
  0x000002109f12d9a0 JavaThread "C1 CompilerThread0" daemon [_thread_blocked, id=9780, stack(0x000000398fc00000,0x000000398fd00000)]
  0x000002109f12ff90 JavaThread "Sweeper thread" daemon [_thread_blocked, id=6072, stack(0x000000398fd00000,0x000000398fe00000)]
  0x000002109fd2a3f0 JavaThread "C1 CompilerThread1" daemon [_thread_blocked, id=18688, stack(0x000000398fe00000,0x000000398ff00000)]
  0x000002109fd58010 JavaThread "C1 CompilerThread2" daemon [_thread_blocked, id=4460, stack(0x000000398ff00000,0x0000003990000000)]
  0x000002109fd61d70 JavaThread "Notification Thread" daemon [_thread_blocked, id=1624, stack(0x0000003990000000,0x0000003990100000)]
  0x000002109fd6a040 JavaThread "Common-Cleaner" daemon [_thread_blocked, id=12992, stack(0x0000003990200000,0x0000003990300000)]
  0x00000210a0e614f0 JavaThread "C1 CompilerThread3" daemon [_thread_blocked, id=9244, stack(0x0000003990f00000,0x0000003991000000)]
  0x00000210a143da80 JavaThread "JNA Cleaner" daemon [_thread_blocked, id=18500, stack(0x0000003991800000,0x0000003991900000)]
  0x00000210a150e910 JavaThread "Worker-Bootstrap-1" daemon [_thread_in_Java, id=14252, stack(0x0000003992900000,0x0000003992a00000)]
  0x00000210a150c290 JavaThread "Worker-Bootstrap-2" daemon [_thread_in_Java, id=9824, stack(0x0000003992a00000,0x0000003992b00000)]
  0x00000210a150cc30 JavaThread "Worker-Bootstrap-3" daemon [_thread_in_Java, id=18636, stack(0x0000003992b00000,0x0000003992c00000)]
  0x00000210a150d100 JavaThread "Worker-Bootstrap-4" daemon [_thread_in_Java, id=7264, stack(0x0000003992c00000,0x0000003992d00000)]
  0x00000210a150ede0 JavaThread "Worker-Bootstrap-5" daemon [_thread_in_Java, id=11704, stack(0x0000003992d00000,0x0000003992e00000)]
  0x00000210a150b8f0 JavaThread "Worker-Bootstrap-6" daemon [_thread_in_Java, id=6608, stack(0x0000003992e00000,0x0000003992f00000)]
  0x00000210a31e0550 JavaThread "Worker-Bootstrap-7" daemon [_thread_in_Java, id=3876, stack(0x0000003992f00000,0x0000003993000000)]
  0x00000210a31e2700 JavaThread "Worker-Bootstrap-8" daemon [_thread_in_Java, id=6688, stack(0x0000003993000000,0x0000003993100000)]
  0x00000210a31dda00 JavaThread "Worker-Bootstrap-9" daemon [_thread_in_Java, id=580, stack(0x0000003993100000,0x0000003993200000)]
  0x00000210a31dcb90 JavaThread "Worker-Bootstrap-10" daemon [_thread_in_Java, id=12300, stack(0x0000003993200000,0x0000003993300000)]
  0x00000210a31e2bd0 JavaThread "Worker-Bootstrap-11" daemon [_thread_in_Java, id=2948, stack(0x0000003993300000,0x0000003993400000)]
  0x00000210a31e3570 JavaThread "Worker-Bootstrap-12" daemon [_thread_in_Java, id=4308, stack(0x0000003993400000,0x0000003993500000)]
  0x00000210a31ded40 JavaThread "Worker-Bootstrap-13" daemon [_thread_in_Java, id=19408, stack(0x0000003993500000,0x0000003993600000)]
  0x00000210a31df6e0 JavaThread "Worker-Bootstrap-14" daemon [_thread_in_Java, id=8728, stack(0x0000003993600000,0x0000003993700000)]
  0x00000210a31dfbb0 JavaThread "Worker-Bootstrap-15" daemon [_thread_in_Java, id=2088, stack(0x0000003993700000,0x0000003993800000)]
  0x00000210a31e3a40 JavaThread "Timer hack thread" daemon [_thread_blocked, id=14300, stack(0x0000003990600000,0x0000003990700000)]
  0x00000210a31e30a0 JavaThread "Keep-Alive-Timer" daemon [_thread_blocked, id=4300, stack(0x0000003990500000,0x0000003990600000)]

Other Threads:
  0x000002109f0ed3e0 VMThread "VM Thread" [stack: 0x000000398f400000,0x000000398f500000] [id=5792]
  0x000002109f168e00 WatcherThread [stack: 0x0000003990100000,0x0000003990200000] [id=11036]
  0x00000210845813e0 GCTaskThread "GC Thread#0" [stack: 0x000000398ef00000,0x000000398f000000] [id=14232]
  0x000002109ffaf2a0 GCTaskThread "GC Thread#1" [stack: 0x0000003990a00000,0x0000003990b00000] [id=19372]
  0x00000210a01a3ee0 GCTaskThread "GC Thread#2" [stack: 0x0000003990b00000,0x0000003990c00000] [id=18708]
  0x00000210a09711e0 GCTaskThread "GC Thread#3" [stack: 0x0000003990c00000,0x0000003990d00000] [id=3336]
  0x00000210a0971490 GCTaskThread "GC Thread#4" [stack: 0x0000003990d00000,0x0000003990e00000] [id=5232]
  0x00000210a060a5a0 GCTaskThread "GC Thread#5" [stack: 0x0000003990e00000,0x0000003990f00000] [id=9376]
  0x00000210a0eda840 GCTaskThread "GC Thread#6" [stack: 0x0000003991000000,0x0000003991100000] [id=18220]
  0x00000210a0edaaf0 GCTaskThread "GC Thread#7" [stack: 0x0000003991100000,0x0000003991200000] [id=19316]
  0x00000210a0edada0 GCTaskThread "GC Thread#8" [stack: 0x0000003991200000,0x0000003991300000] [id=12984]
  0x00000210a0edb050 GCTaskThread "GC Thread#9" [stack: 0x0000003991300000,0x0000003991400000] [id=19008]
  0x00000210a0edbf20 GCTaskThread "GC Thread#10" [stack: 0x0000003991400000,0x0000003991500000] [id=15880]
  0x00000210a2d44be0 GCTaskThread "GC Thread#11" [stack: 0x0000003991700000,0x0000003991800000] [id=14684]
  0x00000210a2d453f0 GCTaskThread "GC Thread#12" [stack: 0x0000003990400000,0x0000003990500000] [id=2080]
  0x00000210845828c0 ConcurrentGCThread "G1 Main Marker" [stack: 0x000000398f000000,0x000000398f100000] [id=10480]
  0x0000021084584820 ConcurrentGCThread "G1 Conc#0" [stack: 0x000000398f100000,0x000000398f200000] [id=19072]
  0x00000210a0edfa30 ConcurrentGCThread "G1 Conc#1" [stack: 0x0000003991500000,0x0000003991600000] [id=16060]
  0x00000210a0f3fc30 ConcurrentGCThread "G1 Conc#2" [stack: 0x0000003991600000,0x0000003991700000] [id=17972]
  0x00000210845ce5f0 ConcurrentGCThread "G1 Refine#0" [stack: 0x000000398f200000,0x000000398f300000] [id=9972]
  0x00000210a424b840 ConcurrentGCThread "G1 Refine#1" [stack: 0x0000003991d00000,0x0000003991e00000] [id=10576]
  0x00000210a424bb20 ConcurrentGCThread "G1 Refine#2" [stack: 0x0000003991e00000,0x0000003991f00000] [id=17936]
  0x00000210a424be00 ConcurrentGCThread "G1 Refine#3" [stack: 0x0000003991f00000,0x0000003992000000] [id=19304]
  0x00000210a424a140 ConcurrentGCThread "G1 Refine#4" [stack: 0x0000003992000000,0x0000003992100000] [id=2884]
  0x00000210a424a9e0 ConcurrentGCThread "G1 Refine#5" [stack: 0x0000003992100000,0x0000003992200000] [id=8988]
  0x00000210a424acc0 ConcurrentGCThread "G1 Refine#6" [stack: 0x0000003992200000,0x0000003992300000] [id=18348]
  0x00000210a5ff6260 ConcurrentGCThread "G1 Refine#7" [stack: 0x0000003992300000,0x0000003992400000] [id=12036]
  0x00000210a5ff6820 ConcurrentGCThread "G1 Refine#8" [stack: 0x0000003992400000,0x0000003992500000] [id=4288]
  0x00000210a5ff84e0 ConcurrentGCThread "G1 Refine#9" [stack: 0x0000003992500000,0x0000003992600000] [id=13356]
  0x00000210a5ff59c0 ConcurrentGCThread "G1 Refine#10" [stack: 0x0000003992600000,0x0000003992700000] [id=17704]
  0x00000210a5ff5120 ConcurrentGCThread "G1 Refine#11" [stack: 0x0000003992700000,0x0000003992800000] [id=18668]
  0x00000210a5ff7960 ConcurrentGCThread "G1 Refine#12" [stack: 0x0000003992800000,0x0000003992900000] [id=12444]
  0x00000210845cedb0 ConcurrentGCThread "G1 Service" [stack: 0x000000398f300000,0x000000398f400000] [id=9292]

Threads with active compile tasks:

VM state: not at safepoint (normal execution)

VM Mutex/Monitor currently owned by a thread: None

Heap address: 0x0000000080000000, size: 2048 MB, Compressed Oops mode: 32-bit

CDS archive(s) not mapped
Compressed class space mapped at: 0x0000000100000000-0x0000000140000000, reserved size: 1073741824
Narrow klass base: 0x0000000000000000, Narrow klass shift: 3, Narrow klass range: 0x140000000

GC Precious Log:
 CPUs: 16 total, 16 available
 Memory: 15754M
 Large Page Support: Disabled
 NUMA Support: Disabled
 Compressed Oops: Enabled (32-bit)
 Heap Region Size: 32M
 Heap Min Capacity: 32M
 Heap Initial Capacity: 256M
 Heap Max Capacity: 2G
 Pre-touch: Disabled
 Parallel Workers: 13
 Concurrent Workers: 3
 Concurrent Refinement Workers: 13
 Periodic GC: Disabled

Heap:
 garbage-first heap   total 1540096K, used 483415K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 9 young (294912K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K

Heap Regions: E=young(eden), S=young(survivor), O=old, HS=humongous(starts), HC=humongous(continues), CS=collection set, F=free, OA=open archive, CA=closed archive, TAMS=top-at-mark-start (previous, next)
|   0|0x0000000080000000, 0x0000000082000000, 0x0000000082000000|100%| O|  |TAMS 0x0000000082000000, 0x0000000080000000| Untracked 
|   1|0x0000000082000000, 0x0000000084000000, 0x0000000084000000|100%| O|  |TAMS 0x0000000084000000, 0x0000000082000000| Untracked 
|   2|0x0000000084000000, 0x0000000086000000, 0x0000000086000000|100%| O|  |TAMS 0x0000000086000000, 0x0000000084000000| Untracked 
|   3|0x0000000086000000, 0x0000000088000000, 0x0000000088000000|100%| O|  |TAMS 0x0000000088000000, 0x0000000086000000| Untracked 
|   4|0x0000000088000000, 0x000000008a000000, 0x000000008a000000|100%| O|  |TAMS 0x000000008a000000, 0x0000000088000000| Untracked 
|   5|0x000000008a000000, 0x000000008c000000, 0x000000008c000000|100%| O|  |TAMS 0x000000008c000000, 0x000000008a000000| Untracked 
|   6|0x000000008c000000, 0x000000008e000000, 0x000000008e000000|100%| O|  |TAMS 0x000000008e000000, 0x000000008c000000| Untracked 
|   7|0x000000008e000000, 0x000000008e000000, 0x0000000090000000|  0%| F|  |TAMS 0x000000008e000000, 0x000000008e000000| Untracked 
|   8|0x0000000090000000, 0x0000000091650000, 0x0000000092000000| 69%| O|  |TAMS 0x0000000090000000, 0x0000000090000000| Untracked 
|   9|0x0000000092000000, 0x0000000092000000, 0x0000000094000000|  0%| F|  |TAMS 0x0000000092000000, 0x0000000092000000| Untracked 
|  10|0x0000000094000000, 0x0000000094000000, 0x0000000096000000|  0%| F|  |TAMS 0x0000000094000000, 0x0000000094000000| Untracked 
|  11|0x0000000096000000, 0x0000000096000000, 0x0000000098000000|  0%| F|  |TAMS 0x0000000096000000, 0x0000000096000000| Untracked 
|  12|0x0000000098000000, 0x0000000098000000, 0x000000009a000000|  0%| F|  |TAMS 0x0000000098000000, 0x0000000098000000| Untracked 
|  13|0x000000009a000000, 0x000000009a000000, 0x000000009c000000|  0%| F|  |TAMS 0x000000009a000000, 0x000000009a000000| Untracked 
|  14|0x000000009c000000, 0x000000009c000000, 0x000000009e000000|  0%| F|  |TAMS 0x000000009c000000, 0x000000009c000000| Untracked 
|  15|0x000000009e000000, 0x000000009e000000, 0x00000000a0000000|  0%| F|  |TAMS 0x000000009e000000, 0x000000009e000000| Untracked 
|  16|0x00000000a0000000, 0x00000000a0000000, 0x00000000a2000000|  0%| F|  |TAMS 0x00000000a0000000, 0x00000000a0000000| Untracked 
|  17|0x00000000a2000000, 0x00000000a2000000, 0x00000000a4000000|  0%| F|  |TAMS 0x00000000a2000000, 0x00000000a2000000| Untracked 
|  18|0x00000000a4000000, 0x00000000a4000000, 0x00000000a6000000|  0%| F|  |TAMS 0x00000000a4000000, 0x00000000a4000000| Untracked 
|  19|0x00000000a6000000, 0x00000000a61c5e60, 0x00000000a8000000|  5%| S|CS|TAMS 0x00000000a6000000, 0x00000000a6000000| Complete 
|  20|0x00000000a8000000, 0x00000000a8000000, 0x00000000aa000000|  0%| F|  |TAMS 0x00000000a8000000, 0x00000000a8000000| Untracked 
|  21|0x00000000aa000000, 0x00000000aa000000, 0x00000000ac000000|  0%| F|  |TAMS 0x00000000aa000000, 0x00000000aa000000| Untracked 
|  22|0x00000000ac000000, 0x00000000ac000000, 0x00000000ae000000|  0%| F|  |TAMS 0x00000000ac000000, 0x00000000ac000000| Untracked 
|  23|0x00000000ae000000, 0x00000000ae000000, 0x00000000b0000000|  0%| F|  |TAMS 0x00000000ae000000, 0x00000000ae000000| Untracked 
|  24|0x00000000b0000000, 0x00000000b0000000, 0x00000000b2000000|  0%| F|  |TAMS 0x00000000b0000000, 0x00000000b0000000| Untracked 
|  25|0x00000000b2000000, 0x00000000b2000000, 0x00000000b4000000|  0%| F|  |TAMS 0x00000000b2000000, 0x00000000b2000000| Untracked 
|  26|0x00000000b4000000, 0x00000000b4000000, 0x00000000b6000000|  0%| F|  |TAMS 0x00000000b4000000, 0x00000000b4000000| Untracked 
|  27|0x00000000b6000000, 0x00000000b6000000, 0x00000000b8000000|  0%| F|  |TAMS 0x00000000b6000000, 0x00000000b6000000| Untracked 
|  28|0x00000000b8000000, 0x00000000b8000000, 0x00000000ba000000|  0%| F|  |TAMS 0x00000000b8000000, 0x00000000b8000000| Untracked 
|  29|0x00000000ba000000, 0x00000000ba000000, 0x00000000bc000000|  0%| F|  |TAMS 0x00000000ba000000, 0x00000000ba000000| Untracked 
|  30|0x00000000bc000000, 0x00000000bc000000, 0x00000000be000000|  0%| F|  |TAMS 0x00000000bc000000, 0x00000000bc000000| Untracked 
|  31|0x00000000be000000, 0x00000000be000000, 0x00000000c0000000|  0%| F|  |TAMS 0x00000000be000000, 0x00000000be000000| Untracked 
|  32|0x00000000c0000000, 0x00000000c0000000, 0x00000000c2000000|  0%| F|  |TAMS 0x00000000c0000000, 0x00000000c0000000| Untracked 
|  33|0x00000000c2000000, 0x00000000c2000000, 0x00000000c4000000|  0%| F|  |TAMS 0x00000000c2000000, 0x00000000c2000000| Untracked 
|  34|0x00000000c4000000, 0x00000000c4000000, 0x00000000c6000000|  0%| F|  |TAMS 0x00000000c4000000, 0x00000000c4000000| Untracked 
|  35|0x00000000c6000000, 0x00000000c6000000, 0x00000000c8000000|  0%| F|  |TAMS 0x00000000c6000000, 0x00000000c6000000| Untracked 
|  36|0x00000000c8000000, 0x00000000c8000000, 0x00000000ca000000|  0%| F|  |TAMS 0x00000000c8000000, 0x00000000c8000000| Untracked 
|  37|0x00000000ca000000, 0x00000000ca000000, 0x00000000cc000000|  0%| F|  |TAMS 0x00000000ca000000, 0x00000000ca000000| Untracked 
|  38|0x00000000cc000000, 0x00000000cc8a8ee8, 0x00000000ce000000| 27%| E|  |TAMS 0x00000000cc000000, 0x00000000cc000000| Complete 
|  39|0x00000000ce000000, 0x00000000d0000000, 0x00000000d0000000|100%| E|CS|TAMS 0x00000000ce000000, 0x00000000ce000000| Complete 
|  40|0x00000000d0000000, 0x00000000d2000000, 0x00000000d2000000|100%| E|CS|TAMS 0x00000000d0000000, 0x00000000d0000000| Complete 
|  41|0x00000000d2000000, 0x00000000d4000000, 0x00000000d4000000|100%| E|CS|TAMS 0x00000000d2000000, 0x00000000d2000000| Complete 
|  47|0x00000000de000000, 0x00000000e0000000, 0x00000000e0000000|100%| E|CS|TAMS 0x00000000de000000, 0x00000000de000000| Complete 
|  48|0x00000000e0000000, 0x00000000e2000000, 0x00000000e2000000|100%| E|CS|TAMS 0x00000000e0000000, 0x00000000e0000000| Complete 
|  49|0x00000000e2000000, 0x00000000e4000000, 0x00000000e4000000|100%| E|CS|TAMS 0x00000000e2000000, 0x00000000e2000000| Complete 
|  50|0x00000000e4000000, 0x00000000e6000000, 0x00000000e6000000|100%| E|CS|TAMS 0x00000000e4000000, 0x00000000e4000000| Complete 
|  51|0x00000000e6000000, 0x00000000e8000000, 0x00000000e8000000|100%| E|CS|TAMS 0x00000000e6000000, 0x00000000e6000000| Complete 

Card table byte_map: [0x0000021097970000,0x0000021097d70000] _byte_map_base: 0x0000021097570000

Marking Bits (Prev, Next): (CMBitMap*) 0x0000021084581790, (CMBitMap*) 0x00000210845817d0
 Prev Bits: [0x0000021098170000, 0x000002109a170000)
 Next Bits: [0x000002109a170000, 0x000002109c170000)

Polling page: 0x0000021083d10000

Metaspace:

Usage:
  Non-class:     54.85 MB used.
      Class:      8.75 MB used.
       Both:     63.60 MB used.

Virtual space:
  Non-class space:       56.00 MB reserved,      55.25 MB ( 99%) committed,  7 nodes.
      Class space:        1.00 GB reserved,       9.06 MB ( <1%) committed,  1 nodes.
             Both:        1.05 GB reserved,      64.31 MB (  6%) committed. 

Chunk freelists:
   Non-Class:  172.00 KB
       Class:  2.89 MB
        Both:  3.06 MB

MaxMetaspaceSize: unlimited
CompressedClassSpaceSize: 1.00 GB
Initial GC threshold: 21.00 MB
Current GC threshold: 105.44 MB
CDS: off
MetaspaceReclaimPolicy: balanced
 - commit_granule_bytes: 65536.
 - commit_granule_words: 8192.
 - virtual_space_node_default_size: 1048576.
 - enlarge_chunks_in_place: 1.
 - new_chunks_are_fully_committed: 0.
 - uncommit_free_chunks: 1.
 - use_allocation_guard: 0.
 - handle_deallocations: 1.


Internal statistics:

num_allocs_failed_limit: 27.
num_arena_births: 1032.
num_arena_deaths: 36.
num_vsnodes_births: 8.
num_vsnodes_deaths: 0.
num_space_committed: 1026.
num_space_uncommitted: 0.
num_chunks_returned_to_freelist: 80.
num_chunks_taken_from_freelist: 3070.
num_chunk_merges: 28.
num_chunk_splits: 2015.
num_chunks_enlarged: 1434.
num_purges: 2.
num_inconsistent_stats: 0.

CodeHeap 'non-profiled nmethods': size=119168Kb used=4278Kb max_used=4577Kb free=114889Kb
 bounds [0x000002108f890000, 0x000002108fd10000, 0x0000021096cf0000]
CodeHeap 'profiled nmethods': size=119104Kb used=8875Kb max_used=10551Kb free=110228Kb
 bounds [0x0000021088440000, 0x0000021088ea0000, 0x000002108f890000]
CodeHeap 'non-nmethods': size=7488Kb used=3672Kb max_used=3694Kb free=3815Kb
 bounds [0x0000021087cf0000, 0x00000210880a0000, 0x0000021088440000]
 total_blobs=7232 nmethods=5717 adapters=1424
 compilation: enabled
              stopped_count=0, restarted_count=0
 full_count=0

Compilation events (20 events):
Event: 6.818 Thread 0x000002109f12d9a0 7488       3       org.lwjgl.system.StructBuffer::sizeof (8 bytes)
Event: 6.818 Thread 0x00000210a0e614f0 7489       3       org.lwjgl.glfw.GLFWVidMode$Buffer::getElementFactory (5 bytes)
Event: 6.819 Thread 0x00000210a0e614f0 nmethod 7489 0x0000021088bffb10 code [0x0000021088bffca0, 0x0000021088bffe18]
Event: 6.819 Thread 0x00000210a0e614f0 7490       3       org.lwjgl.glfw.GLFWVidMode$Buffer::getElementFactory (4 bytes)
Event: 6.819 Thread 0x000002109fd2a3f0 nmethod 7486 0x0000021088d45790 code [0x0000021088d45920, 0x0000021088d45a38]
Event: 6.819 Thread 0x000002109fd58010 nmethod 7487 0x0000021088c2d990 code [0x0000021088c2db40, 0x0000021088c2dda8]
Event: 6.819 Thread 0x000002109f12d9a0 nmethod 7488 0x0000021088d46110 code [0x0000021088d462c0, 0x0000021088d46518]
Event: 6.819 Thread 0x000002109fd2a3f0 7491       3       org.lwjgl.glfw.GLFWVidMode::sizeof (4 bytes)
Event: 6.819 Thread 0x00000210a0e614f0 nmethod 7490 0x0000021088d86d10 code [0x0000021088d86ea0, 0x0000021088d86fb8]
Event: 6.819 Thread 0x000002109fd2a3f0 nmethod 7491 0x0000021088dd6490 code [0x0000021088dd6620, 0x0000021088dd6738]
Event: 6.835 Thread 0x00000210a0e614f0 7492       1       edg::c (5 bytes)
Event: 6.835 Thread 0x000002109fd58010 7493       1       edg::d (5 bytes)
Event: 6.835 Thread 0x000002109f12d9a0 7494       1       edg::e (5 bytes)
Event: 6.835 Thread 0x000002109fd58010 nmethod 7493 0x000002108fa69610 code [0x000002108fa697a0, 0x000002108fa69878]
Event: 6.835 Thread 0x00000210a0e614f0 nmethod 7492 0x000002108fa69310 code [0x000002108fa694a0, 0x000002108fa69578]
Event: 6.836 Thread 0x000002109f12d9a0 nmethod 7494 0x000002108fa69010 code [0x000002108fa691a0, 0x000002108fa69278]
Event: 7.026 Thread 0x000002109fd58010 7497       3       java.util.concurrent.ForkJoinPool$WorkQueue::getSlot (9 bytes)
Event: 7.026 Thread 0x00000210a0e614f0 7498       3       java.lang.invoke.VarHandleReferences$Array::getAcquire (49 bytes)
Event: 7.027 Thread 0x00000210a0e614f0 nmethod 7498 0x000002108898d890 code [0x000002108898daa0, 0x000002108898e1c8]
Event: 7.027 Thread 0x000002109fd58010 nmethod 7497 0x0000021088c80310 code [0x0000021088c805a0, 0x0000021088c811a8]

GC Heap History (20 events):
Event: 6.618 GC heap before
{Heap before GC invocations=54 (full 0):
 garbage-first heap   total 1540096K, used 1136612K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 64700K, committed 65408K, reserved 1105920K
  class space    used 8889K, committed 9216K, reserved 1048576K
}
Event: 6.621 GC heap after
{Heap after GC invocations=55 (full 0):
 garbage-first heap   total 1540096K, used 253013K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 64700K, committed 65408K, reserved 1105920K
  class space    used 8889K, committed 9216K, reserved 1048576K
}
Event: 6.697 GC heap before
{Heap before GC invocations=55 (full 0):
 garbage-first heap   total 1540096K, used 1137749K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65020K, committed 65664K, reserved 1105920K
  class space    used 8946K, committed 9280K, reserved 1048576K
}
Event: 6.700 GC heap after
{Heap after GC invocations=56 (full 0):
 garbage-first heap   total 1540096K, used 253315K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65020K, committed 65664K, reserved 1105920K
  class space    used 8946K, committed 9280K, reserved 1048576K
}
Event: 6.776 GC heap before
{Heap before GC invocations=56 (full 0):
 garbage-first heap   total 1540096K, used 1138051K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65020K, committed 65664K, reserved 1105920K
  class space    used 8946K, committed 9280K, reserved 1048576K
}
Event: 6.778 GC heap after
{Heap after GC invocations=57 (full 0):
 garbage-first heap   total 1540096K, used 253523K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65020K, committed 65664K, reserved 1105920K
  class space    used 8946K, committed 9280K, reserved 1048576K
}
Event: 6.854 GC heap before
{Heap before GC invocations=57 (full 0):
 garbage-first heap   total 1540096K, used 1138259K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 6.855 GC heap after
{Heap after GC invocations=58 (full 0):
 garbage-first heap   total 1540096K, used 253585K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 6.932 GC heap before
{Heap before GC invocations=58 (full 0):
 garbage-first heap   total 1540096K, used 1138321K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 6.934 GC heap after
{Heap after GC invocations=59 (full 0):
 garbage-first heap   total 1540096K, used 253534K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.010 GC heap before
{Heap before GC invocations=59 (full 0):
 garbage-first heap   total 1540096K, used 1138270K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.012 GC heap after
{Heap after GC invocations=60 (full 0):
 garbage-first heap   total 1540096K, used 253532K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65124K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.089 GC heap before
{Heap before GC invocations=60 (full 0):
 garbage-first heap   total 1540096K, used 1138268K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.090 GC heap after
{Heap after GC invocations=61 (full 0):
 garbage-first heap   total 1540096K, used 253667K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.167 GC heap before
{Heap before GC invocations=61 (full 0):
 garbage-first heap   total 1540096K, used 1138403K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.168 GC heap after
{Heap after GC invocations=62 (full 0):
 garbage-first heap   total 1540096K, used 253742K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.241 GC heap before
{Heap before GC invocations=62 (full 0):
 garbage-first heap   total 1540096K, used 1138478K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.242 GC heap after
{Heap after GC invocations=63 (full 0):
 garbage-first heap   total 1540096K, used 253867K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.315 GC heap before
{Heap before GC invocations=63 (full 0):
 garbage-first heap   total 1540096K, used 1138603K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 28 young (917504K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}
Event: 7.317 GC heap after
{Heap after GC invocations=64 (full 0):
 garbage-first heap   total 1540096K, used 253879K [0x0000000080000000, 0x0000000100000000)
  region size 32768K, 1 young (32768K), 1 survivors (32768K)
 Metaspace       used 65125K, committed 65856K, reserved 1105920K
  class space    used 8962K, committed 9280K, reserved 1048576K
}

Deoptimization events (20 events):
Event: 6.563 Thread 0x000002108454c450 Uncommon trap: trap_request=0xffffffd6 fr.pc=0x000002108fa2c068 relative=0x0000000000000348
Event: 6.563 Thread 0x000002108454c450 Uncommon trap: reason=array_check action=maybe_recompile pc=0x000002108fa2c068 method=java.util.Arrays.fill([Ljava/lang/Object;Ljava/lang/Object;)V @ 13 c2
Event: 6.563 Thread 0x000002108454c450 DEOPT PACKING pc=0x000002108fa2c068 sp=0x000000398eefe260
Event: 6.563 Thread 0x000002108454c450 DEOPT UNPACKING pc=0x0000021087d423a3 sp=0x000000398eefe220 mode 2
Event: 6.597 Thread 0x000002108454c450 Uncommon trap: trap_request=0xffffff45 fr.pc=0x000002108fb3ccac relative=0x00000000000006cc
Event: 6.597 Thread 0x000002108454c450 Uncommon trap: reason=unstable_if action=reinterpret pc=0x000002108fb3ccac method=it.unimi.dsi.fastutil.ints.Int2ObjectOpenHashMap.find(I)I @ 91 c2
Event: 6.597 Thread 0x000002108454c450 DEOPT PACKING pc=0x000002108fb3ccac sp=0x000000398eefeda0
Event: 6.597 Thread 0x000002108454c450 DEOPT UNPACKING pc=0x0000021087d423a3 sp=0x000000398eefecf8 mode 2
Event: 6.597 Thread 0x000002108454c450 Uncommon trap: trap_request=0xffffff45 fr.pc=0x000002108fc415f4 relative=0x00000000000002d4
Event: 6.597 Thread 0x000002108454c450 Uncommon trap: reason=unstable_if action=reinterpret pc=0x000002108fc415f4 method=java.lang.invoke.AbstractValidatingLambdaMetafactory.isAdaptableTo(Ljava/lang/Class;Ljava/lang/Class;Z)Z @ 81 c2
Event: 6.597 Thread 0x000002108454c450 DEOPT PACKING pc=0x000002108fc415f4 sp=0x000000398eefdce0
Event: 6.597 Thread 0x000002108454c450 DEOPT UNPACKING pc=0x0000021087d423a3 sp=0x000000398eefdc70 mode 2
Event: 6.598 Thread 0x000002108454c450 Uncommon trap: trap_request=0xffffff45 fr.pc=0x000002108fcac834 relative=0x00000000000017b4
Event: 6.598 Thread 0x000002108454c450 Uncommon trap: reason=unstable_if action=reinterpret pc=0x000002108fcac834 method=java.lang.invoke.TypeConvertingMethodAdapter.convertType(Ljava/lang/Class;Ljava/lang/Class;Ljava/lang/Class;)V @ 186 c2
Event: 6.598 Thread 0x000002108454c450 DEOPT PACKING pc=0x000002108fcac834 sp=0x000000398eefdb90
Event: 6.598 Thread 0x000002108454c450 DEOPT UNPACKING pc=0x0000021087d423a3 sp=0x000000398eefdb40 mode 2
Event: 6.598 Thread 0x000002108454c450 Uncommon trap: trap_request=0xffffff45 fr.pc=0x000002108fb39564 relative=0x0000000000000144
Event: 6.598 Thread 0x000002108454c450 Uncommon trap: reason=unstable_if action=reinterpret pc=0x000002108fb39564 method=it.unimi.dsi.fastutil.ints.Int2ObjectOpenHashMap.find(I)I @ 91 c2
Event: 6.598 Thread 0x000002108454c450 DEOPT PACKING pc=0x000002108fb39564 sp=0x000000398eefed60
Event: 6.598 Thread 0x000002108454c450 DEOPT UNPACKING pc=0x0000021087d423a3 sp=0x000000398eefecf0 mode 2

Classes unloaded (18 events):
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054e800 'java/lang/invoke/LambdaForm$DMH+0x000000010054e800'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054e400 'java/lang/invoke/LambdaForm$DMH+0x000000010054e400'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054e000 'java/lang/invoke/LambdaForm$DMH+0x000000010054e000'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054dc00 'java/lang/invoke/LambdaForm$DMH+0x000000010054dc00'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054d800 'java/lang/invoke/LambdaForm$DMH+0x000000010054d800'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054d400 'java/lang/invoke/LambdaForm$DMH+0x000000010054d400'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054d000 'java/lang/invoke/LambdaForm$DMH+0x000000010054d000'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054c800 'java/lang/invoke/LambdaForm$DMH+0x000000010054c800'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054c400 'java/lang/invoke/LambdaForm$DMH+0x000000010054c400'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x000000010054c000 'java/lang/invoke/LambdaForm$DMH+0x000000010054c000'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100546c00 'java/lang/invoke/LambdaForm$DMH+0x0000000100546c00'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100546800 'java/lang/invoke/LambdaForm$DMH+0x0000000100546800'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100546400 'java/lang/invoke/LambdaForm$DMH+0x0000000100546400'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100545c00 'java/lang/invoke/LambdaForm$DMH+0x0000000100545c00'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100546000 'java/lang/invoke/LambdaForm$DMH+0x0000000100546000'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100545400 'java/lang/invoke/LambdaForm$DMH+0x0000000100545400'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100545000 'java/lang/invoke/LambdaForm$DMH+0x0000000100545000'
Event: 5.983 Thread 0x000002109f0ed3e0 Unloading class 0x0000000100544c00 'java/lang/invoke/LambdaForm$DMH+0x0000000100544c00'

Classes redefined (0 events):
No events

Internal exceptions (20 events):
Event: 5.572 Thread 0x000002108454c450 Implicit null exception at 0x000002108f9b3e99 to 0x000002108f9b4293
Event: 5.584 Thread 0x000002108454c450 Exception <a 'sun/nio/fs/WindowsException'{0x00000000c98699a8}> (0x00000000c98699a8) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\prims\jni.cpp, line 516]
Event: 5.593 Thread 0x000002108454c450 Exception <a 'java/lang/IncompatibleClassChangeError'{0x00000000c07bd2d0}: Found class java.lang.Object, but interface was expected> (0x00000000c07bd2d0) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 833]
Event: 6.199 Thread 0x000002108454c450 Implicit null exception at 0x000002108f94f968 to 0x000002108f94fae8
Event: 6.557 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000df8601e8}: 'java.lang.Object java.lang.invoke.DirectMethodHandle$Holder.invokeStatic(java.lang.Object, java.lang.Object, double)'> (0x00000000df8601e8) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.563 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000d1e9a618}: 'java.lang.Object java.lang.invoke.DirectMethodHandle$Holder.invokeStatic(java.lang.Object, java.lang.Object, int, int)'> (0x00000000d1e9a618) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.564 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000cf14ba30}: 'int java.lang.invoke.DirectMethodHandle$Holder.invokeStatic(java.lang.Object)'> (0x00000000cf14ba30) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.584 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000bc076900}: 'double java.lang.invoke.DirectMethodHandle$Holder.invokeStatic(java.lang.Object, int)'> (0x00000000bc076900) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.595 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000b71c8f30}: 'java.lang.Object java.lang.invoke.DirectMethodHandle$Holder.invokeSpecial(java.lang.Object, java.lang.Object, java.lang.Object, int, java.lang.Object)'> (0x00000000b71c8f30) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.595 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000b71cc618}: 'java.lang.Object java.lang.invoke.Invokers$Holder.linkToTargetMethod(java.lang.Object, int, java.lang.Object, java.lang.Object)'> (0x00000000b71cc618) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.598 Thread 0x000002108454c450 Implicit null exception at 0x000002108fcab411 to 0x000002108fcac81b
Event: 6.613 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000ab9b3180}: 'int java.lang.invoke.DirectMethodHandle$Holder.invokeStaticInit(java.lang.Object)'> (0x00000000ab9b3180) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.614 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000a944e358}: 'int java.lang.invoke.Invokers$Holder.invokeExact_MT(java.lang.Object, java.lang.Object)'> (0x00000000a944e358) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.626 Thread 0x000002108454c450 Exception <a 'sun/nio/fs/WindowsException'{0x00000000e7ac6380}> (0x00000000e7ac6380) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\prims\jni.cpp, line 516]
Event: 6.626 Thread 0x000002108454c450 Exception <a 'sun/nio/fs/WindowsException'{0x00000000e7ac66e0}> (0x00000000e7ac66e0) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\prims\jni.cpp, line 516]
Event: 6.640 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000d0a92618}: 'java.lang.Object java.lang.invoke.DirectMethodHandle$Holder.invokeInterface(java.lang.Object, java.lang.Object, double)'> (0x00000000d0a92618) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.780 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000e6fe48d8}: 'long java.lang.invoke.DirectMethodHandle$Holder.invokeInterface(java.lang.Object, java.lang.Object)'> (0x00000000e6fe48d8) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.788 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000e0878fd0}: 'java.lang.Object java.lang.invoke.DirectMethodHandle$Holder.newInvokeSpecial(java.lang.Object, long)'> (0x00000000e0878fd0) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.840 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000b3f31b10}: 'void java.lang.invoke.DirectMethodHandle$Holder.invokeSpecial(java.lang.Object, java.lang.Object, int, long)'> (0x00000000b3f31b10) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]
Event: 6.842 Thread 0x000002108454c450 Exception <a 'java/lang/NoSuchMethodError'{0x00000000b1d99e00}: 'void java.lang.invoke.DirectMethodHandle$Holder.invokeStatic(java.lang.Object, int, long)'> (0x00000000b1d99e00) 
thrown [d:\a\_work\1\jdk\src\hotspot\share\interpreter\linkResolver.cpp, line 766]

VM Operations (20 events):
Event: 6.618 Executing VM operation: G1CollectForAllocation
Event: 6.621 Executing VM operation: G1CollectForAllocation done
Event: 6.697 Executing VM operation: G1CollectForAllocation
Event: 6.703 Executing VM operation: G1CollectForAllocation done
Event: 6.776 Executing VM operation: G1CollectForAllocation
Event: 6.778 Executing VM operation: G1CollectForAllocation done
Event: 6.854 Executing VM operation: G1CollectForAllocation
Event: 6.855 Executing VM operation: G1CollectForAllocation done
Event: 6.932 Executing VM operation: G1CollectForAllocation
Event: 6.936 Executing VM operation: G1CollectForAllocation done
Event: 7.010 Executing VM operation: G1CollectForAllocation
Event: 7.012 Executing VM operation: G1CollectForAllocation done
Event: 7.089 Executing VM operation: G1CollectForAllocation
Event: 7.091 Executing VM operation: G1CollectForAllocation done
Event: 7.167 Executing VM operation: G1CollectForAllocation
Event: 7.168 Executing VM operation: G1CollectForAllocation done
Event: 7.241 Executing VM operation: G1CollectForAllocation
Event: 7.242 Executing VM operation: G1CollectForAllocation done
Event: 7.315 Executing VM operation: G1CollectForAllocation
Event: 7.317 Executing VM operation: G1CollectForAllocation done

Events (20 events):
Event: 6.483 loading class sun/net/www/protocol/http/HttpURLConnection$HttpInputStream
Event: 6.484 loading class sun/net/www/protocol/http/HttpURLConnection$HttpInputStream done
Event: 6.484 loading class java/util/Collections$UnmodifiableSortedMap
Event: 6.484 loading class java/util/Collections$UnmodifiableSortedMap done
Event: 6.485 loading class sun/net/www/http/KeepAliveCache$1
Event: 6.485 loading class sun/net/www/http/KeepAliveCache$1 done
Event: 6.485 Thread 0x00000210a31e30a0 Thread added: 0x00000210a31e30a0
Event: 6.485 loading class sun/net/www/http/ClientVector
Event: 6.485 loading class sun/net/www/http/ClientVector done
Event: 6.496 loading class sun/net/www/http/KeepAliveEntry
Event: 6.496 loading class sun/net/www/http/KeepAliveEntry done
Event: 6.499 Thread 0x00000210a3645330 Thread exited: 0x00000210a3645330
Event: 6.508 loading class sun/reflect/generics/repository/FieldRepository
Event: 6.508 loading class sun/reflect/generics/repository/FieldRepository done
Event: 6.520 loading class jdk/internal/vm/annotation/ForceInline
Event: 6.521 loading class jdk/internal/vm/annotation/ForceInline done
Event: 6.613 loading class java/lang/invoke/DirectMethodHandle$StaticAccessor
Event: 6.613 loading class java/lang/invoke/DirectMethodHandle$StaticAccessor done
Event: 6.637 loading class java/util/function/DoubleFunction
Event: 6.637 loading class java/util/function/DoubleFunction done


Dynamic libraries:
0x00007ff7b1190000 - 0x00007ff7b119e000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\javaw.exe
0x00007fff62890000 - 0x00007fff62aa4000 	C:\WINDOWS\SYSTEM32\ntdll.dll
0x00007fff61b40000 - 0x00007fff61c03000 	C:\WINDOWS\System32\KERNEL32.DLL
0x00007fff5fcd0000 - 0x00007fff6006c000 	C:\WINDOWS\System32\KERNELBASE.dll
0x00007fff60510000 - 0x00007fff60621000 	C:\WINDOWS\System32\ucrtbase.dll
0x00007fff569d0000 - 0x00007fff569e8000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\jli.dll
0x00007fff588e0000 - 0x00007fff588fb000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\VCRUNTIME140.dll
0x00007fff62020000 - 0x00007fff621cd000 	C:\WINDOWS\System32\USER32.dll
0x00007fff60250000 - 0x00007fff60276000 	C:\WINDOWS\System32\win32u.dll
0x00007fff618f0000 - 0x00007fff61919000 	C:\WINDOWS\System32\GDI32.dll
0x00007fff45490000 - 0x00007fff4571e000 	C:\WINDOWS\WinSxS\amd64_microsoft.windows.common-controls_6595b64144ccf1df_6.0.22621.608_none_a9444ca7c10bb01d\COMCTL32.dll
0x00007fff60070000 - 0x00007fff60183000 	C:\WINDOWS\System32\gdi32full.dll
0x00007fff62530000 - 0x00007fff625d7000 	C:\WINDOWS\System32\msvcrt.dll
0x00007fff603f0000 - 0x00007fff6048a000 	C:\WINDOWS\System32\msvcp_win.dll
0x00007fff60850000 - 0x00007fff60881000 	C:\WINDOWS\System32\IMM32.DLL
0x00007fff58920000 - 0x00007fff5892c000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\vcruntime140_1.dll
0x00007fff202f0000 - 0x00007fff2037d000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\msvcp140.dll
0x00007ffedfd20000 - 0x00007ffee097d000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\server\jvm.dll
0x00007fff61570000 - 0x00007fff6161e000 	C:\WINDOWS\System32\ADVAPI32.dll
0x00007fff62400000 - 0x00007fff624a4000 	C:\WINDOWS\System32\sechost.dll
0x00007fff621d0000 - 0x00007fff622e5000 	C:\WINDOWS\System32\RPCRT4.dll
0x00007fff61c20000 - 0x00007fff61c28000 	C:\WINDOWS\System32\PSAPI.DLL
0x00007fff588a0000 - 0x00007fff588a9000 	C:\WINDOWS\SYSTEM32\WSOCK32.dll
0x00007fff54560000 - 0x00007fff54594000 	C:\WINDOWS\SYSTEM32\WINMM.dll
0x00007fff56270000 - 0x00007fff5627a000 	C:\WINDOWS\SYSTEM32\VERSION.dll
0x00007fff62380000 - 0x00007fff623f1000 	C:\WINDOWS\System32\WS2_32.dll
0x00007fff5ed20000 - 0x00007fff5ed38000 	C:\WINDOWS\SYSTEM32\kernel.appcore.dll
0x00007fff586a0000 - 0x00007fff586aa000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\jimage.dll
0x00007fff58d70000 - 0x00007fff58f9e000 	C:\WINDOWS\SYSTEM32\DBGHELP.DLL
0x00007fff61c30000 - 0x00007fff61fb9000 	C:\WINDOWS\System32\combase.dll
0x00007fff61620000 - 0x00007fff616f7000 	C:\WINDOWS\System32\OLEAUT32.dll
0x00007fff573d0000 - 0x00007fff57402000 	C:\WINDOWS\SYSTEM32\dbgcore.DLL
0x00007fff60490000 - 0x00007fff6050b000 	C:\WINDOWS\System32\bcryptPrimitives.dll
0x00007fff56200000 - 0x00007fff56225000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\java.dll
0x00007fff55fa0000 - 0x00007fff55fb8000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\zip.dll
0x00007ffee8710000 - 0x00007ffee87e7000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\jsvml.dll
0x00007fff608f0000 - 0x00007fff610e0000 	C:\WINDOWS\System32\SHELL32.dll
0x00007fff5dce0000 - 0x00007fff5e5ae000 	C:\WINDOWS\SYSTEM32\windows.storage.dll
0x00007fff5dba0000 - 0x00007fff5dcde000 	C:\WINDOWS\SYSTEM32\wintypes.dll
0x00007fff61a40000 - 0x00007fff61b31000 	C:\WINDOWS\System32\SHCORE.dll
0x00007fff61fc0000 - 0x00007fff6201e000 	C:\WINDOWS\System32\shlwapi.dll
0x00007fff5fc00000 - 0x00007fff5fc21000 	C:\WINDOWS\SYSTEM32\profapi.dll
0x00007fff3fdd0000 - 0x00007fff3fde9000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\net.dll
0x00007fff5a620000 - 0x00007fff5a74f000 	C:\WINDOWS\SYSTEM32\WINHTTP.dll
0x00007fff5f190000 - 0x00007fff5f1f9000 	C:\WINDOWS\system32\mswsock.dll
0x00007fff3fdb0000 - 0x00007fff3fdc6000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\nio.dll
0x00007fff3fda0000 - 0x00007fff3fda9000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\management.dll
0x00007fff3b590000 - 0x00007fff3b59b000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\management_ext.dll
0x00007fff56be0000 - 0x00007fff56bf7000 	C:\WINDOWS\system32\napinsp.dll
0x00007fff56bc0000 - 0x00007fff56bdb000 	C:\WINDOWS\system32\pnrpnsp.dll
0x00007fff5e830000 - 0x00007fff5e923000 	C:\WINDOWS\SYSTEM32\DNSAPI.dll
0x00007fff5e800000 - 0x00007fff5e82d000 	C:\WINDOWS\SYSTEM32\IPHLPAPI.DLL
0x00007fff61c10000 - 0x00007fff61c19000 	C:\WINDOWS\System32\NSI.dll
0x00007fff228a0000 - 0x00007fff228b1000 	C:\WINDOWS\System32\winrnr.dll
0x00007fff58b60000 - 0x00007fff58b75000 	C:\WINDOWS\system32\wshbth.dll
0x00007ffefe5e0000 - 0x00007ffefe601000 	C:\WINDOWS\system32\nlansp_c.dll
0x00007fff5a160000 - 0x00007fff5a16a000 	C:\Windows\System32\rasadhlp.dll
0x00007fff59b70000 - 0x00007fff59bf3000 	C:\WINDOWS\System32\fwpuclnt.dll
0x00007fff5f3f0000 - 0x00007fff5f40b000 	C:\WINDOWS\SYSTEM32\CRYPTSP.dll
0x00007fff5ec90000 - 0x00007fff5ecc5000 	C:\WINDOWS\system32\rsaenh.dll
0x00007fff5f290000 - 0x00007fff5f2b8000 	C:\WINDOWS\SYSTEM32\USERENV.dll
0x00007fff5f600000 - 0x00007fff5f628000 	C:\WINDOWS\SYSTEM32\bcrypt.dll
0x00007fff5f410000 - 0x00007fff5f41c000 	C:\WINDOWS\SYSTEM32\CRYPTBASE.dll
0x00007fff5a170000 - 0x00007fff5a189000 	C:\WINDOWS\SYSTEM32\dhcpcsvc6.DLL
0x00007fff59fd0000 - 0x00007fff59fef000 	C:\WINDOWS\SYSTEM32\dhcpcsvc.DLL
0x00007fff3b4f0000 - 0x00007fff3b530000 	C:\Users\Jacob\AppData\Local\Temp\jna-71328959\jna9947952542743476989.dll
0x00007fff61700000 - 0x00007fff6189c000 	C:\WINDOWS\System32\Ole32.dll
0x00007fff606a0000 - 0x00007fff60750000 	C:\WINDOWS\System32\clbcatq.dll
0x00007fff4fa70000 - 0x00007fff4fa8d000 	C:\WINDOWS\SYSTEM32\amsi.dll
0x00007fff4f890000 - 0x00007fff4f93e000 	C:\Program Files\Norton Security\Engine\22.20.5.40\symamsi.dll
0x00007fff60630000 - 0x00007fff6069b000 	C:\WINDOWS\System32\WINTRUST.dll
0x00007fff60280000 - 0x00007fff603e6000 	C:\WINDOWS\System32\CRYPT32.dll
0x00007fff5f9d0000 - 0x00007fff5f9e2000 	C:\WINDOWS\SYSTEM32\MSASN1.dll
0x00007ffeec400000 - 0x00007ffeec450000 	C:\WINDOWS\SYSTEM32\Pdh.dll
0x00007fff3ca50000 - 0x00007fff3ca60000 	C:\WINDOWS\System32\perfos.dll
0x00007fff5d2a0000 - 0x00007fff5d2b0000 	C:\WINDOWS\SYSTEM32\pfclient.dll
0x00007fff3b580000 - 0x00007fff3b590000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\verify.dll
0x00007ffeec030000 - 0x00007ffeec0a5000 	C:\Users\Jacob\AppData\Local\Temp\lwjglJacob\3.3.1-build-7\lwjgl.dll
0x00007ffee36b0000 - 0x00007ffee3909000 	C:\Users\Jacob\AppData\Local\Temp\lwjglJacob\3.3.1-build-7\jemalloc.dll
0x00007fff3b4e0000 - 0x00007fff3b4ed000 	C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\sunmscapi.dll
0x00007fff5f5d0000 - 0x00007fff5f5fd000 	C:\WINDOWS\SYSTEM32\ncrypt.dll
0x00007fff5f590000 - 0x00007fff5f5c7000 	C:\WINDOWS\SYSTEM32\NTASN1.dll
0x00007fff20280000 - 0x00007fff202e1000 	C:\Users\Jacob\AppData\Local\Temp\lwjglJacob\3.3.1-build-7\glfw.dll
0x00007fff39280000 - 0x00007fff392c6000 	C:\WINDOWS\SYSTEM32\dinput8.dll
0x00007fff3b340000 - 0x00007fff3b351000 	C:\WINDOWS\SYSTEM32\xinput1_4.dll
0x00007fff5f950000 - 0x00007fff5f99e000 	C:\WINDOWS\SYSTEM32\cfgmgr32.dll
0x00007fff5f920000 - 0x00007fff5f94c000 	C:\WINDOWS\SYSTEM32\DEVOBJ.dll
0x00007fff5d500000 - 0x00007fff5d52b000 	C:\WINDOWS\SYSTEM32\dwmapi.dll
0x00007fff5d2d0000 - 0x00007fff5d37b000 	C:\WINDOWS\system32\uxtheme.dll
0x00007fff2e500000 - 0x00007fff2e639000 	C:\ProgramData\A-Volute\A-Volute.Nahimic\Modules\Scheduled\x64\AudioDevProps2.dll
0x00007fff4b1d0000 - 0x00007fff4b3d1000 	C:\WINDOWS\SYSTEM32\inputhost.dll
0x00007fff5cf60000 - 0x00007fff5d093000 	C:\WINDOWS\SYSTEM32\CoreMessaging.dll
0x00000210a51e0000 - 0x00000210a52fe000 	C:\WINDOWS\System32\MSCTF.dll
0x00007ffee8020000 - 0x00007ffee8120000 	C:\WINDOWS\SYSTEM32\opengl32.dll
0x00007fff3b310000 - 0x00007fff3b33d000 	C:\WINDOWS\SYSTEM32\GLU32.dll
0x00007fff5d3b0000 - 0x00007fff5d3e6000 	C:\WINDOWS\SYSTEM32\dxcore.dll
0x00007fff575f0000 - 0x00007fff57639000 	C:\WINDOWS\SYSTEM32\directxdatabasehelper.dll
0x00007fff2e450000 - 0x00007fff2e47d000 	C:\WINDOWS\System32\DriverStore\FileRepository\u0386435.inf_amd64_b30f12ffb4d24f80\B385286\atig6pxx.dll
0x00007ffecbd30000 - 0x00007ffecf9bb000 	C:\WINDOWS\System32\DriverStore\FileRepository\u0386435.inf_amd64_b30f12ffb4d24f80\B385286\atio6axx.dll
0x00007fff610f0000 - 0x00007fff61564000 	C:\WINDOWS\System32\SETUPAPI.dll

dbghelp: loaded successfully - version: 4.0.5 - missing functions: none
symbol engine: initialized successfully - sym options: 0x614 - pdb path: .;C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin;C:\WINDOWS\SYSTEM32;C:\WINDOWS\WinSxS\amd64_microsoft.windows.common-controls_6595b64144ccf1df_6.0.22621.608_none_a9444ca7c10bb01d;C:\Users\Jacob\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-gamma\windows-x64\java-runtime-gamma\bin\server;C:\Users\Jacob\AppData\Local\Temp\jna-71328959;C:\Program Files\Norton Security\Engine\22.20.5.40;C:\Users\Jacob\AppData\Local\Temp\lwjglJacob\3.3.1-build-7;C:\ProgramData\A-Volute\A-Volute.Nahimic\Modules\Scheduled\x64;C:\WINDOWS\System32\DriverStore\FileRepository\u0386435.inf_amd64_b30f12ffb4d24f80\B385286

VM Arguments:
jvm_args: -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Dos.name=Windows 10 -Dos.version=10.0 -Xss1M -Djava.library.path=C:\Users\Jacob\AppData\Roaming\.minecraft\bin\44685878b69bb36a6fb05390c06c8b0243d34f57 -Dminecraft.launcher.brand=minecraft-launcher -Dminecraft.launcher.version=2.3.645 -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M -Dlog4j.configurationFile=C:\Users\Jacob\AppData\Roaming\.minecraft\assets\log_configs\client-1.12.xml 
java_command: net.minecraft.client.main.Main --username DatBoiCheeks --version 1.19.3 --gameDir C:\Users\Jacob\AppData\Roaming\.minecraft --assetsDir C:\Users\Jacob\AppData\Roaming\.minecraft\assets --assetIndex 2 --uuid a8c1aefee98b4677b783dc1beb0b04bc -heuVB5ZQTRgGhrTuT1-YufL5tQ --clientId NWVmYjhkZDktNjEzZi00ZjNmLTlkZDgtMjBjNmNlZWMzNDBl --xuid 2535432210837001 --userType msa --versionType release
java_class_path (initial): C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\github\oshi\oshi-core\6.2.2\oshi-core-6.2.2.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\google\code\gson\gson\2.10\gson-2.10.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\google\guava\failureaccess\1.0.1\failureaccess-1.0.1.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\google\guava\guava\31.1-jre\guava-31.1-jre.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\ibm\icu\icu4j\71.1\icu4j-71.1.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\authlib\3.16.29\authlib-3.16.29.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\blocklist\1.0.10\blocklist-1.0.10.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\brigadier\1.0.18\brigadier-1.0.18.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\datafixerupper\5.0.28\datafixerupper-5.0.28.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\javabridge\2.0.25\javabridge-2.0.25.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\logging\1.1.1\logging-1.1.1.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\patchy\2.2.10\patchy-2.2.10.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\text2speech\1.13.9\text2speech-1.13.9.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\com\mojang\text2speech\1.13.9\text2speech-1.13.9-natives-windows.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\commons-codec\commons-codec\1.15\commons-codec-1.15.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\commons-io\commons-io\2.11.0\commons-io-2.11.0.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\commons-logging\commons-logging\1.2\commons-logging-1.2.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\io\netty\netty-buffer\4.1.82.Final\netty-buffer-4.1.82.Final.jar;C:\Users\Jacob\AppData\Roaming\.minecraft\libraries\io\netty\netty-codec\4.1.82.Final\netty-c
Launcher Type: SUN_STANDARD

[Global flags]
     intx CICompilerCount                          = 12                                        {product} {ergonomic}
     uint ConcGCThreads                            = 3                                         {product} {ergonomic}
     uint G1ConcRefinementThreads                  = 13                                        {product} {ergonomic}
     uint G1EagerReclaimRemSetThreshold            = 256                                  {experimental} {ergonomic}
   size_t G1HeapRegionSize                         = 33554432                                  {product} {command line}
    uintx G1NewSizePercent                         = 20                                   {experimental} {command line}
    uintx G1ReservePercent                         = 20                                        {product} {command line}
    uintx GCDrainStackTargetSize                   = 64                                        {product} {ergonomic}
    ccstr HeapDumpPath                             = MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump         {manageable} {command line}
   size_t InitialHeapSize                          = 268435456                                 {product} {ergonomic}
   size_t MarkStackSize                            = 4194304                                   {product} {ergonomic}
    uintx MaxGCPauseMillis                         = 50                                        {product} {command line}
   size_t MaxHeapSize                              = 2147483648                                {product} {command line}
   size_t MaxNewSize                               = 1275068416                                {product} {ergonomic}
   size_t MinHeapDeltaBytes                        = 33554432                                  {product} {ergonomic}
   size_t MinHeapSize                              = 33554432                                  {product} {ergonomic}
    uintx NonNMethodCodeHeapSize                   = 7602480                                {pd product} {ergonomic}
    uintx NonProfiledCodeHeapSize                  = 122027880                              {pd product} {ergonomic}
    uintx ProfiledCodeHeapSize                     = 122027880                              {pd product} {ergonomic}
    uintx ReservedCodeCacheSize                    = 251658240                              {pd product} {ergonomic}
     bool SegmentedCodeCache                       = true                                      {product} {ergonomic}
   size_t SoftMaxHeapSize                          = 2147483648                             {manageable} {ergonomic}
     intx ThreadStackSize                          = 1024                                   {pd product} {command line}
     bool UnlockExperimentalVMOptions              = true                                 {experimental} {command line}
     bool UseCompressedClassPointers               = true                           {product lp64_product} {ergonomic}
     bool UseCompressedOops                        = true                           {product lp64_product} {ergonomic}
     bool UseG1GC                                  = true                                      {product} {command line}
     bool UseLargePagesIndividualAllocation        = false                                  {pd product} {ergonomic}

Logging:
Log output configuration:
 #0: stdout all=warning uptime,level,tags
 #1: stderr all=off uptime,level,tags

Environment Variables:
PATH=C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Users\Jacob\AppData\Local\Microsoft\WindowsApps
USERNAME=Jacob
OS=Windows_NT
PROCESSOR_IDENTIFIER=AMD64 Family 25 Model 80 Stepping 0, AuthenticAMD



---------------  S Y S T E M  ---------------

OS:
 Windows 11 , 64 bit Build 22621 (10.0.22621.1344)
OS uptime: 0 days 0:18 hours

CPU: total 16 (initial active 16) (16 cores per cpu, 2 threads per core) family 25 model 80 stepping 0 microcode 0x0, cx8, cmov, fxsr, ht, mmx, 3dnowpref, sse, sse2, sse3, ssse3, sse4a, sse4.1, sse4.2, popcnt, lzcnt, tsc, tscinvbit, avx, avx2, aes, erms, clmul, bmi1, bmi2, adx, sha, fma, vzeroupper, clflush, clflushopt

Memory: 4k page, system-wide physical 15754M (8703M free)
TotalPageFile size 18698M (AvailPageFile size 10181M)
current process WorkingSet (physical memory assigned to process): 1732M, peak: 1894M
current process commit charge ("private bytes"): 1832M, peak: 1991M

vm_info: OpenJDK 64-Bit Server VM (17.0.3+7-LTS) for windows-amd64 JRE (17.0.3+7-LTS), built on Apr 20 2022 04:24:16 by "" with MS VC++ 16.10 / 16.11 (VS2019)

END.
