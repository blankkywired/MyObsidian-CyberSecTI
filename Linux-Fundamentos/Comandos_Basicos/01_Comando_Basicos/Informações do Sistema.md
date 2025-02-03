#01_Comandos_Basicos


| **Command** |                                                               **Description**                                                                |
| ----------- | :------------------------------------------------------------------------------------------------------------------------------------------: |
| `whoami`    |                                               Mostra o nome do atual usuario logado na maquina                                               |
| `id`        |                                                            Returns users identity                                                            |
| `hostname`  |                                             exibe o nome do computador que o usuario está logado                                             |
| `uname`     | Mostra as principais informações basicas do sistema e do hardware como distribuição linux, nome do hostname, arquitetura do processador etc. |
| `pwd`       |                                                       Returns working directory name.                                                        |
| `ifconfig`  |      The ifconfig utility is used to assign or to view an address to a network interface and/or configure network interface parameters.      |
| `ip`        |                           Ip is a utility to show or manipulate routing, network devices, interfaces and tunnels.                            |
| `netstat`   |                                                            Shows network status.                                                             |
| `ss`        |                                                   Another utility to investigate sockets.                                                    |
| `ps`        |                                                            Shows process status.                                                             |
| `who`       |                                                          Displays who is logged in.                                                          |
| `env`       |                                               Prints environment or sets and executes command.                                               |
| `lsblk`     |                                                             Lists block devices.                                                             |
| `lsusb`     |                                                              Lists USB devices                                                               |
| `lsof`      |                                                             Lists opened files.                                                              |
| `lspci`     |                                                              Lists PCI devices.                                                              |

#### Whoami
mostra o nome do atual usuario logado na maquina

```shell-session
cry0l1t3@htb[/htb]$ whoami

cry0l1t3
```

#### Uname 
Uname -a 
mostra todas informações basicas do sistema

```shell-session
cry0l1t3@htb[/htb]$ uname -a

Linux box 4.15.0-99-generic #100-Ubuntu SMP Wed Apr 22 20:32:56 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux
```

**Kernel** : Linux
**Distro**: Ubuntu
**edição do kernel lançado** :  4.15.0-99-generic 
**modelo de arquitetura do processador** :  x86_64  

#### lscpu
Lista as informações de hardware da cpu, como por exemplo:

Arquitetura da cpu
quantidade de nucleos 
frequencia
quantidade de sockets
Nome do modelo do processador
```shell-session
blankky@blankky-Inspiron-15-3520:~$ lscpu
Architecture:             x86_64
  CPU op-mode(s):         32-bit, 64-bit
  Address sizes:          39 bits physical, 48 bits virtual
  Byte Order:             Little Endian
CPU(s):                   12
  On-line CPU(s) list:    0-11
Vendor ID:                GenuineIntel
  Model name:             12th Gen Intel(R) Core(TM) i5-1235U
    CPU family:           6
    Model:                154
    Thread(s) per core:   2
    Core(s) per socket:   10
    Socket(s):            1
    Stepping:             4
    CPU(s) scaling MHz:   21%
    CPU max MHz:          4400,0000
    CPU min MHz:          400,0000
    BogoMIPS:             4992,00
    Flags:                fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm 
                          pbe syscall nx pdpe1gb rdtscp lm constant_tsc art arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid ap
                          erfmperf tsc_known_freq pni pclmulqdq dtes64 monitor ds_cpl vmx smx est tm2 ssse3 sdbg fma cx16 xtpr pdcm sse4_1 sse
                          4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm 3dnowprefetch cpuid_fault epb ssbd 
                          ibrs ibpb stibp ibrs_enhanced tpr_shadow flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms i
                          nvpcid rdseed adx smap clflushopt clwb intel_pt sha_ni xsaveopt xsavec xgetbv1 xsaves split_lock_detect user_shstk a
                          vx_vnni dtherm ida arat pln pts hwp hwp_notify hwp_act_window hwp_epp hwp_pkg_req hfi vnmi umip pku ospke waitpkg gf
                          ni vaes vpclmulqdq rdpid movdiri movdir64b fsrm md_clear serialize arch_lbr ibt flush_l1d arch_capabilities
Virtualisation features:  
  Virtualisation:         VT-x
Caches (sum of all):      
  L1d:                    352 KiB (10 instances)
  L1i:                    576 KiB (10 instances)
  L2:                     6,5 MiB (4 instances)
  L3:                     12 MiB (1 instance)
NUMA:                     
  NUMA node(s):           1
  NUMA node0 CPU(s):      0-11
Vulnerabilities:          
  Gather data sampling:   Not affected
  Itlb multihit:          Not affected
  L1tf:                   Not affected
  Mds:                    Not affected
  Meltdown:               Not affected
  Mmio stale data:        Not affected
  Reg file data sampling: Mitigation; Clear Register File
  Retbleed:               Not affected
  Spec rstack overflow:   Not affected
  Spec store bypass:      Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:             Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:             Mitigation; Enhanced / Automatic IBRS; IBPB conditional; RSB filling; PBRSB-eIBRS SW sequence; BHI BHI_DIS_S
  Srbds:                  Not affected
```