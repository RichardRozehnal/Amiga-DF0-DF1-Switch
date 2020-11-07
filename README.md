# Amiga DF0 / DF1 Switch

Naprostá většina her na Amigu jde bootovat (spouštět) pouze z interní floppy mechaniky DF0. Pokud máte třeba emulátor floppy mechaniky Gotek připojeny externě jako DF1 a chcete z něj spouštet hry a programy, musíte Amigu donutit myslet si, že ona externí mechanika je DF0. To se udělá tak, že se na základní desce Amigy u IC 8520 (CIA-B) prohodí piny (vývody) signálů SEL0 a SEL1. Tyto piny se odpájí od desky a SEL0 se přivede na desku tam, kde byl SEL1 a SEL1 tam kde byl SEL0. Potom si bude Amiga myslet, že externí mechanika je DF0 a dovolí z ní bootovat. Tím se interní mechanika deaktivuje a nepůjde používat.

U A1000, A2000, A2000CR, A500, A500 Plus, CDTV, A3000, A3000T jsou signály SEL0 a SEL1 na pinech 13 a 14.
U A600, A1200, A4000 jsou signály SEL0 a SEL1 na pinech 15 a 16.

Pokud budete na prohození pinů vytvářet přepínač, tak je nutné přepínat pouze při vypnuté Amize! Jinak hrozí poškození čipu.