# System 3 / Foresight: p_hit latch analysis

An interactive report that asks whether a frozen vision-language model (Qwen3-VL-8B in System 3) knows *when* proactive events happen on the OmniPro benchmark. It covers the 932 samples where audio is not required (none + helpful).

Main finding: p_hit latches. The model detects the first event sharply and then stays high, so later events become invisible. Most of this is a saturation problem rather than a perception one: when p_hit is still low just before the second event, the second event produces a clear jump.

Open `index.html`. It is served with GitHub Pages.

Video frames come from OmniPro (CC BY-NC 4.0) and are shown for research purposes only.
