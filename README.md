Shadowsocks for Windows
=======================

[中文说明]

Important note
--------------
This project has been forked from its original repository on August 22nd 2015,
shortly after fellow GitHub user @clowwindy has been asked by Beijing Central
Government to remove everything of the shadowsocks project.

Since then, this project has not been maintained by me or others, but many
forks happened to spread the code; each maintained with different quality and
purpose. However, as nobody oversees these projects, nobody should trust or rely
on these forked projects.

You can clearly see and proof that I forked the shadowsocks projects directly
from the original author, just before he had to close most of his projects.
Feel free to use his code for your own adaptions or to learn how your government
tries to protect you from dangerous ideas, like alternate beliefs, the disease
to speek freely (which infested the whole western hemisphere) or the joy of sex
and watching others having sex.

My thoughts and prayers extend to everyone fighting for a better future for
their society as well as to every victim of arbitrary province lords
incarcerating the workers class in the name of the workers class' party.

Never give up <3

__ Herzmut,
Berlin, Oct 16 '16


#### Features

1. System proxy configuration
2. PAC mode and global mode
3. [GFWList] and user rules
4. Supports HTTP proxy
5. Supports server auto switching
6. Supports UDP relay (see Usage)

#### Download

Download the [latest release].

#### Basic

1. Find Shadowsocks icon in the notification tray
2. You can add multiple servers in servers menu
3. Select `Enable System Proxy` menu to enable system proxy. Please disable other
proxy addons in your browser, or set them to use system proxy
4. You can also configure your browser proxy manually if you don't want to enable
system proxy. Set Socks5 or HTTP proxy to 127.0.0.1:1080. You can change this
port in `Servers -> Edit Servers`

#### PAC

1. You can change PAC rules by editing the PAC file. When you save the PAC file
with any editor, Shadowsocks will notify browsers about the change automatically
2. You can also update PAC file from [GFWList] \(maintained by 3rd party)
3. You can also use online PAC URL

#### Server Auto Switching

1. Load balance: choosing server randomly
2. High availability: choosing the best server (low latency and packet loss)
3. Choose By Total Package Loss: ping and choose. Please also enable
   `Availability Statistics` in the menu if you want to use this
4. Write your own strategy by implement IStrategy interface and send us a pull request!

#### UDP

For UDP, you need to use SocksCap or ProxyCap to force programs you want
to be proxied to tunnel over Shadowsocks

#### Multiple Instances

If you want to manage multiple servers using other tools like SwitchyOmega,
you can start multiple Shadowsocks instances. To avoid configuration conflicts,
copy Shadowsocks to a new directory and choose a different local port.

#### Global hotkeys

Hotkeys are NOT registered automatically. You should re-register all hotkeys after
restarting Shadowsocks. If you are using multiple instances of Shadowsocks,
you must set different key combination for other instances.

##### How to input?

1. Put focus in the corresponding textbox.
2. Press the key combination that you want to use.
3. Release all keys when you think it is ready.
4. Your input appears in the textbox.

##### How to change?

1. Put focus in the corresponding textbox.
2. Press BackSpace key to clear content.
3. Re-input new key combination.

##### How to deactivate?

1. Clear content in the textbox that you want to deactivate,
if you want to deactivate all, please clear all textboxes.
2. Press OK button to confirm.

##### Meaning of label color

- Green: This key combination is not occupied by other programs and register successfully.
- Yellow: This key combination is occupied by other programs and you have to change to another one.
- Transparent without color: The initial status.

#### Server Configuration

Please visit [Servers] for more information.

#### Portable Mode

If you want to put all temporary files into shadowsocks/temp folder instead of
system temp folder, create a `shadowsocks_portable_mode.txt` into shadowsocks folder.

#### Develop

[Visual Studio 2015] & [.NET Framework 4.6.2 Developer Pack] are required.

#### License

GPLv3


[Appveyor]:       https://ci.appveyor.com/project/wongsyrone/shadowsocks-windows-pljx3
[Build Status]:   https://ci.appveyor.com/api/projects/status/otie4km27ws1wak2/branch/master?svg=true
[latest release]: https://github.com/shadowsocks/shadowsocks-csharp/releases
[GFWList]:        https://github.com/gfwlist/gfwlist
[Servers]:        https://github.com/shadowsocks/shadowsocks/wiki/Ports-and-Clients#linux--server-side
[中文说明]:       https://github.com/shadowsocks/shadowsocks-windows/wiki/Shadowsocks-Windows-%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E
[Visual Studio 2015]: https://www.visualstudio.com/downloads/
[.NET Framework 4.6.2 Developer Pack]: https://www.microsoft.com/download/details.aspx?id=53321