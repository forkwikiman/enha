이 문서는 [Bochs](Bochs.md) 항목의 bochsrc.txt에 대한 하위문서입니다.

Bochs 설정파일의 세부적 내용을 알아보기로 한다. 원문 설정파일을 보자. 한글번역도 덧붙였다. (아래 글을 복사하여
bochsrc.txt로 저장하면 설정파일로 사용이 가능하다.)  
'#' 이 주석문구이다. 구문을 활성화 하려면 주석을 지우자.

* * *

# Bochs에 몇 메가바이트의 용량을 RAM으로 사용하게 할것입니까?

megs: 64

# count=설정할 CPU의 갯수 ips=CPU의 대략적인 속도

cpu: count=1, ips=1200000, reset_on_triple_fault=1, ignore_bad_msrs=1

# ROM이미지 설정 (절대 건드리지 말것!)

romimage: file=BIOS-bochs-latest  
vgaromimage: file=VGABIOS-lgpl-latest  
vga: extension=cirrus, update_freq=25  
pci: enabled=1, chipset=i440fx, slot1=cirrus

# 어떤 플로피디스크 이미지를 사용할 것입니까?  

#floppya: 1_44=floppya.img, status=inserted

#floppyb: 1_44=floppyb.img, status=inserted

# 예를들어 SDL폴더안의 ABCD.IMG 라는 플로피이미지를 플로피디스크A에 적용하고 싶다면

# 'floppya: 1_44=ABCD.IMG, status=inserted' 로 설정하면 됩니다.

#플로피디스크는 잘 사용하지 않으니, 기본설정에서는 비활성화 되어 있습니다. 활성화 하려면 구문앞의 # 을 제거하세요.

ata0: enabled=1, ioaddr1=0x1f0, ioaddr2=0x3f0, irq=14

ata1: enabled=1, ioaddr1=0x170, ioaddr2=0x370, irq=15

# ATA장치는 ATA3 까지 설정가능하고, 이론적으로 총 4개의 ATA를 사용하능하고, slave까지 모두 사용하면 총 8개의
CD,하드디스크 사용이 가능합니다.

# ATA장치를 더 많이 사용하려면 ATA값을 추가하여야 합니다. 값은 아래에 있습니다.

# ata0: enabled=1, ioaddr1=0x1f0, ioaddr2=0x3f0, irq=14  
# ata1: enabled=1, ioaddr1=0x170, ioaddr2=0x370, irq=15  
# ata2: enabled=1, ioaddr1=0x1e8, ioaddr2=0x3e0, irq=11  
# ata3: enabled=1, ioaddr1=0x168, ioaddr2=0x360, irq=9

# 같은 ata의 master 와 slave 가 동시에 존재해서는 안됩니다!  
# type=□□□□에 들어가는 내용은 하드디스크의 경우에는 disk 를 입력하고, CD의 경우에는 cdrom 을 입력합니다.  
# path="□□□□.□□□" 는 설정할 파일의 이름입니다. 똑같이 맞춰서 설정해야합니다. 확장자도 설정합시다.  
# 만약에 장치를 설정했을때 그 장치의 파일이 이름이 다르거나, 파일이 없으면 Bochs가 튕깁니다. 유의하세요.

ata0-master: type=disk, path="c.img"

#ata0-master: type=cdrom, path="cd.ISO", status=inserted

#ata0-slave: type=disk, path="d.img", model=Android_Bochs

ata1-master: type=disk, mode=vvfat, path=/sdcard/hdd, journal=vvfat.redolog,
model=Mobailism

#ata1-slave: type=cdrom, path="cd.ISO", status=inserted

# slave 장치를 추가하려면 ata□-slave: type=□□□□, path="□□□□.□□□" 로 설정하면 됩니다.  
# 이때, 빈 네모안의 내용은 전부 파일의 이름, 설정할 장치에 맞게 입력하세요!

#아래의 문구는 CD이미지 설정을 위한 문구 형식입니다.  
#꼭 아래의 형식과 같게 설정하세요.

#type=cdrom, path="CD이미지의 이름.ISO", status=inserted

# 예를 들어 CD-ROM에서 부팅하려면 이미 설정되어 있던 ATA0 Master를  
# 비활성화 시키고,

# ata0-master:  
type=cdrom, path="CD이미지의 이름.ISO", status=inserted

# 를 붙여넣기 하고, 부팅설정에서 cdrom으로 맞춰놓으면 됩니다.

# 부팅할 장치를 설정하세요.  
# 하드디스크 부팅은 c 나 disk, CD부팅은 cdrom, 플로피디스크 부팅은 a 나 floppy 입니다.

boot: c

config_interface: textconfig  
#config_interface: wx

#display_library: x

# 다른 선택사항들: win32 sdl wx carbon amigaos beos macintosh nogui rfb term svga 를
선택할 수 있습니다.

# 어느 파일에 로그 메시지를 저장할까요?

log: bochsout.txt

# 활성화 시키려면 놔두고, 비활성화 시키려면 구문앞에 # 을 붙이면 됩니다.  

sb16: midimode=1, wavemode=1, dmatimer=5000

# 기본설정은 활성화 되어있습니다. 굳이 비활성화 시킬 필요는 없는것 같네요.  
# 비활성화는 구문앞에 # 을 붙입니다.

mouse: enabled=1

# 키 맵핑

# However, the key mapping tables are used in the paste function, so  
# in the DLX Linux example I'm enabling keyboard_mapping so that paste  
# will work. Cut&Paste is currently implemented on win32 and X windows only.

#keyboard_mapping: enabled=1, map=$BXSHARE/keymaps/x11-pc-us.map  
#keyboard_mapping: enabled=1, map=$BXSHARE/keymaps/x11-pc-fr.map  
#keyboard_mapping: enabled=1, map=$BXSHARE/keymaps/x11-pc-de.map  
#keyboard_mapping: enabled=1, map=$BXSHARE/keymaps/x11-pc-es.map

