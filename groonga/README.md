This module is an example building Groonga OSv image.

Currently, only `groonga --version` is working.

Otherwise, you will encounter following issue:

```log
/usr/lib/libgroonga.so.0: failed looking up symbol pthread_mutexattr_setpshared

[backtrace]
0x0000000000344430 <elf::object::symbol(unsigned int)+208>
0x00000000003447be <elf::object::resolve_pltgot(unsigned int)+126>
0x00000000003449a6 <elf_resolve_pltgot+54>
0x0000000000390a5e <???+3738206>
0x00000000004411af <???+4460975>
0x0000100001198b24 <???+18451236>
0x000010000119bd46 <???+18464070>
0x000010000119c0f2 <???+18465010>
0x000010000119c21e <grn_hash_create+297>
0x000010000104de59 <???+17096281>
0x000010000104f557 <grn_init+1880>
0x0000100000c10430 <???+12649520>
0x0000000000413f7e <osv::application::run_main(std::string, int, char**)+398>
0x0000000000416088 <osv::application::run_main()+568>
0x000000000020c133 <osv::application::main()+83>
0x0000000000416438 <???+4285496>
0x000000000043fac5 <???+4455109>
0x00000000003efe97 <thread_main_c+39>
0x0000000000391da5 <???+3743141>
```