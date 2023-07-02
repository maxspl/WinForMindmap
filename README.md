# WinForMindmap

Windows forensics mindmap composed of personal notes and other mindmaps, including :
  - some of SANS: https://www.sans.org/blog/the-ultimate-list-of-sans-cheat-sheets/
  - Michel de CREVOISIER evtx mind maps: https://github.com/mdecrevoisier/Microsoft-eventlog-mindmap

This is not a guide for forensic windows, but simply centralized knowledge. So, to find out what to look for on a system, don't hesitate to use the SANS cheat sheets (included in the mindmap).

The mindmap consists of two pages: forensic artifacts and tools. Note that not all of Eric Zimmerman's tools are in the mindmap, so keep in mind that for most artifacts, there's a tool made by E. Zimmerman https://ericzimmerman.github.io/#!index.md.
In fact, there are other pages still under construction, not to be considered.

It's easier to use the mindmap via xmind (.xmind file is in the archive), especially to be able to CTRL + F.
However, a png version is still available.

![Alt text](/assets/Windows_Forensic.png)
![Alt text](/assets/Windows_Forensic_tools.png)

## Usage

Let's say you're analyzing a disk copy of a compromised Windows 10 workstation and want to look for evidence of lateral movements with psexec.

The first step is to search the SANS cheat sheets to find out which artifacts might be useful for proving lateral movement:
![Alt text](/assets/step1.png)

The SANS Hunt Evil cheat sheet indicates that ShimCache may contain traces of psexec.
![Alt text](/assets/step2.png)

For details on this artifact, open the dedicated section of the mindmap:
![Alt text](/assets/step3.png)

Now that we know where the file is and what it contains, we can find a tool to parse it in the Tools sheet.
![Alt text](/assets/step4.png)