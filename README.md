# ICS Easy for Windows

ICS Easy is an offline Windows application for ham radio (amateur radio) net control operators. Log station traffic and print it on ICS forms. This public repository provides installer downloads and instructions. The application source remains private.

## Download and install

1. Open [Releases](https://github.com/mikewi777/ics-easy-downloads/releases).
2. Choose **ICS Easy 1.5.3 - Windows review build** and download **ICS-Easy-1.5.3-Windows-x64-Setup.exe** from Assets.
3. Optionally download **SHA256SUMS.txt** and compare the installer's SHA-256 checksum before running it. This is the current checksum; **SHA256SUMS-original-filename.txt** is historical and is not needed for the current download.
4. Run the installer on Windows x64 and follow its prompts.

The installer is **unsigned** and this is a **pre-release/local-review build**, not a fully validated production release. Windows may show an unknown-publisher or SmartScreen warning. Only install if you trust the source and have verified the download. Clean-machine testing and code signing have not been completed.

GitHub also generates "Source code" ZIP and tar.gz links. Those archives contain this repository's documentation, not the ICS Easy application source or Windows installer.

## Version 1.5.3

- Communications-tower icon and matching version identifiers.
- Red X next to Utilities with an explicit shutdown warning.
- Graceful shutdown waits for pending saves and preserves autosaved drafts.
- Stops its own local server without closing the browser or other applications.
- Blocks shutdown if another registered tab, a save failure, or unsaved non-draft/queue text could cause data loss.

A crashed or suspended tab, or a failed close message, may conservatively block shutdown. No automatic expiry or force-stop feature is included. Review saved work and exported forms before operational use.

## Form sources and third-party components

- ICS 213 and ICS 214: [FEMA ICS forms](https://training.fema.gov/emiweb/is/icsresource/icsforms.html).
- ICS 309: [ARES-SC December 2017 station communications log](https://ares-sc.org/wp-content/uploads/2021/11/ICS-309-Station-Comm-Log-Fillable.pdf), listed on the [ARES-SC downloads page](https://ares-sc.org/downloads/) under **"Download and use as you please"**.
- Bundled runtime and dependency license notices, including pypdf and time-zone data, remain with the installed application. Their respective licenses continue to apply.

Form attribution does not imply endorsement by FEMA, ARES-SC, or another agency. This repository does not grant an open-source license for ICS Easy.
