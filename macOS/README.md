# macOS

I've been a mac user for over 10 years and now heavily relies on Apple
ecosystem. 

I try to keep my setup as minimal as possible. I stick with built-in apps
whenever it possible. First of all, they are good enough for me, and second - 
because they are part of Apple ecosystem they support all cool features, like
[Continuity]. I also install apps via AppStore whenever possible.

[Continuity]: https://www.apple.com/macos/continuity/

## Apps

### Safari

My main browser for everyday surfing. I don't use any extensions for it.

#### Some tips:

- [Page preview] - killer feature
- Use `⌘ + /` to toggle full link preview displayed in the bottom left corner
- Any page can be saved to Apple Books as a PDF via Share menu.

[Page preview]: https://www.igeeksblog.com/how-to-preview-web-page-in-safari-on-mac/

### Quicklook

Quicklook preview is the reason I love macOS so much. I use several plugins
with it:

- [QLColorCode] - preview source code with syntax highlighting
- [qlstephen] - preview files without extensions
- [QLVideo] - preview media (e.g. webm, mkv)

[QLColorCode]: https://github.com/anthonygelibert/QLColorCode
[qlstephen]: https://github.com/whomwah/qlstephen
[QLVideo]: https://github.com/Marginal/QLVideo

I also wrote [QLColorCodeThemer] to change QLColorCode color style based
on macOS theme. I use `base16/eighties` for a Dark mode and `base16/one-light`
with light theme.

[QLColorCodeThemer]: https://github.com/unmade/QLColorCodeThemer

### Terminal

I use standard macOS terminal with [my own theme] for it.

<img src="https://i.imgur.com/R8IkLwK.png" alt="terminal" width="682">

Since macOS Catalina I've switched to [Zsh] as my main shell.

[my own theme]: https://github.com/unmade/terminal-in-rainbows
[zsh]: http://zsh.sourceforge.net

### Notable Mentions

- [DjView] - relatively good open source `djvu` viewer, it can also export
  documents to PDF
- [Fanny] - allows you to monitor CPU/GPU temperature and fans speed 
- [Intel Power Gadget] - a tool to monitor your CPU
- [Raw Photo Processor (RPP)] - a RAW converter to work with colors
- [SlowQuitApps] - prevent you accidentally pressing `⌘ + Q`
- [Serviio] - a programm to stream movis from mac to SmartTV
- [Transmission] - simple BitTorrent client
- [TunnelBlick] - a great OpenVPN client for macOS
- [VLC] - this is what I use to watch movies

[DjView]: http://djvu.sourceforge.net
[Fanny]: https://www.fannywidget.com
[Intel Power Gadget]: https://software.intel.com/en-us/articles/intel-power-gadget
[Raw Photo Processor (RPP)]: https://www.raw-photo-processor.com/RPP/Overview.html
[Serviio]: https://serviio.org
[SlowQuitApps]: https://github.com/dteoh/SlowQuitApps
[Transmission]: https://transmissionbt.com
[TunnelBlick]: https://tunnelblick.net
[VLC]: https://www.videolan.org/vlc/index.html

## Notes

### Remote access

You can access another mac from your mac. The other mac should [enable file
sharing].

[enable file sharing]: https://support.apple.com/guide/mac-help/set-up-file-sharing-on-mac-mh17131/mac

Use these commands:

- `smb://192.168.255.255` - to mount shared mac in Finder
- `vnc://192.168.255.255` - for Screen Sharing

### Working with NTFS

From time to time you need to work with NTFS HDD. The best option would be
to use [Paragon], there is another freeware app called [Mounty].

[Paragon NTFS]: https://www.paragon-software.com/home/ntfs-mac/
[Mounty]: https://mounty.app

## Links

- [Development of Apple's original Macintosh](https://www.folklore.org/index.py)
