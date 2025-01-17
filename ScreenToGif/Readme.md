# ScreenToGif  

This is the current project of ScreenToGif.  

_VS 2019 and .Net 4.8 or newer required._

## What's new? (Version 2.34)

• Added option to manually check for updates (@MaledongGit).  

### Fixed:

♦ The frame navigation using keyboard arrows and home/end buttons was not working.  
♦ If you loaded two editors with a project, the frame list of the first one was being overwritten.  
♦ The keyboard navigation of the screen recorder (newer or older variants) was out of order (@pawlos).  
♦ Some shortcut key were not working for the screen recorder actions (@pawlos).   
♦ Disabled Gifski on x86, since it's unsupported (@MaledongGit).  
♦ Added progress info when processing frames at start and made it possible to cancel during a task (@pawlos).  
♦ The option to cancel a frame altering process was not appearing if the editor already loaded something before.
♦ The text displayed at startup when an update was available was not being updated when the application language had changed.    

### Known Bugs:
  
♠ When exporting with FFmpeg, the last frame may be out of sync with the timmings of the project.  
♠ Cancelling a encoding of FFmpeg will result in a crash (file in use).  
♠ Keystrokes has a 1 pixel transparent border at the bottom-right sides when using a high DPI screen.  
♠ The newer recorder doesn't let you move the selected region to other windows.  
♠ When using the capture option "Capture a frame only when something changes on screen" and moving the recording window, the recording will glitch.  
♠ The Previous/Next repeat buttons are only triggering the events once (because of the command).   
♠ Capturing with DirectX using a screen not in landscaped mode results in a rotated frame.