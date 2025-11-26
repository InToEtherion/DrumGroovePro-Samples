DrumGroovePro - Drum Samples

# DrumGroovePro Drum Samples

This repository contains the drum kit samples used in DrumGroovePro.

---

## 📦 Contents

### Salamander Drumkit
Professional acoustic drum samples

- 400+ WAV files (44.1kHz, 16-bit)
- Multiple velocity layers
- Round-robin variations
- Complete drum kit coverage
- Total size: ~500MB

### MuldjordKit
Professional acoustic drum samples (Tama Superstar)

- Multi-channel WAV files (16 channels)
- Multiple velocity layers
- Round-robin variations
- Metal/Rock drum kit style
- Originally recorded in 2010



  **Modifications:**
- Original: 16-channel WAV files (~2.4GB) for multi-mic mixing
- Modified: Extracted stereo (channels 0-1: AmbL/AmbR) for direct playback (~300MB)
- Files were compressed and uploaded here.

**Conversion command used:**
```bash
find . -name "*.wav" -exec sh -c '
    temp=$(mktemp).wav
    ffmpeg -y -i "$1" -af "pan=stereo|c0=c0|c1=c1" "$temp" 2>/dev/null && mv "$temp" "$1"
' _ {} \;

---

## 📜 Licenses

### Salamander Drumkit
Licensed under **Creative Commons Attribution 3.0 Unported (CC-BY 3.0)**

✅ Commercial use allowed  
✅ Modification allowed  
✅ Distribution allowed  
⚠️ Attribution required

### MuldjordKit
Licensed under **Creative Commons Attribution 4.0 International (CC-BY 4.0)**

✅ Commercial use allowed  
✅ Modification allowed  
✅ Distribution allowed  
⚠️ Attribution required

See `LICENSE.txt` for full license texts.

---

## 👤 Credits

### Salamander Drumkit
- **Original Creator:** Alexander Holm
- **Year:** 2012
- **Source:** http://freepats.zenvoid.org/Percussion/salamander-drumkit.html
- **Website:** https://sfzinstruments.github.io/drums/salamander/

### MuldjordKit
- **Original Creator:** Lars Muldjord
- **Year Recorded:** 2010
- **Source:** https://drumgizmo.org/wiki/doku.php?id=kits:muldjordkit
- **Website:** http://www.muldjord.com

#### MuldjordKit Attribution Requirement
As per the license (January 2021 onwards):
> "Drum samples provided by DrumGizmo.org"

This attribution should appear in album credits or similar liner notes. If album credits aren't available, attribution may be omitted.

---

See `CREDITS.txt` for detailed attribution information.
