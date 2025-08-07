# the killer

为了适应nvgt0.90.0dev的新变化，做出以下调整。

* 1.更改服务端**player.nvgt**的player类中的bool using;变量，由于和nvgt冲突，暂时改为bool using_1;

* 2. 由于3d音频系统的函数变化，重新写了3d音频系统的开关。

* 3. 现在默认pack_files类没有list_file方法，如果想列出文件需要写出：cast<pack_file@>(sound_default_pack).list_files();

* 4. 创建了一个新的包创建器来创建最新的包文件，其中可以对包文件进行加密，之前的包创建器以在最新版nvgt不可用。