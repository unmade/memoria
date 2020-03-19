# macOS

I've been a mac user for over 10 years and now heavily relies on Apple
ecosystem. 

I try to keep my setup as minimal as possible. I stick with built-in apps
whenever it possible. First of all, they are good enough for me, and second - 
because they are part of Apple ecosystem they support all cool features, like
[Continuity]. I also install apps with AppStore whenever possible.

[Continuity]: https://www.apple.com/macos/continuity/

## Apps

### Safari

My main browser for everyday surfing. I don't use any extensions for it.

#### Some tips:

- [Link preview] - killer feature
- Use `⌘ + /` to toggle full link displayed in the bottom left corner
- Any page can be saved to Apple Books as a PDF via Share menu.

### Terminal

I use standard macOS terminal with [my own theme] for it.

<img src="https://i.imgur.com/R8IkLwK.png" alt="terminal" width="682">

Since macOS Catalina I've switched to [Zsh] as my main shell.

[my own theme]: https://github.com/unmade/terminal-in-rainbows
[zsh]: http://zsh.sourceforge.net

### Notable Mentions

- [DjView] - relatively good open source `djvu` viewer, it can also export
  documents to PDF
- [Intel Power Gadget] - a tool to monitor your CPU
- [Raw Photo Processor (RPP)] - a RAW converter to work with colors
- [Serviio] - a programm to stream movis from mac to SmartTV
- [Transmission] - simple BitTorrent client
- [TunnelBlick] - a great OpenVPN client for macOS
- [VLC] - this is what I use to watch movies

[DjView]: http://djvu.sourceforge.net
[Intel Power Gadget]: https://software.intel.com/en-us/articles/intel-power-gadget
[Raw Photo Processor (RPP)]: https://www.raw-photo-processor.com/RPP/Overview.html
[Serviio]: https://serviio.org
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
