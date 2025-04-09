---
layout: default
grand_parent: Jailbreaking Your Kindle
parent: Post Jailbreak
title: Installing KOReader
nav_order: 5
---

# Installing KOReader

_KOReader is a document viewer for E Ink devices. Supported formats include EPUB, PDF, DjVu, XPS, CBT, CBZ, FB2, PDB, TXT, HTML, RTF, CHM, DOC, MOBI and ZIP files._

{: .warning }
Your Kindle must be jailbroken and have MRPI and KUAL installed to be able to run KOReader.

<div id="guide">
    <div class="buttons">
        <button class="btn btn-orange" id="prev">Previous Step</button>
        <span id="stepCounter"></span>
        <button class="btn btn-green" id="next">Next Step</button>
    </div>
    <div id="stepwrapper" class="stepwrapper">
        <div class="step">
            <h2>Determine your firmware version</h2>
            <div class="stepContent">
                <p>Before proceeding, check your Kindle's firmware version by going to:</p>
                <p><strong>Home → Menu → Settings → Menu → Device Info</strong></p>
                <p class="highlight">Different firmware versions require different KOReader packages</p>
            </div>
        </div>
        
        <div class="step">
            <h2>Download KOReader</h2>
            <div class="stepContent">
                <div class="version-block">
                    <p class="version-label">Firmware <=5.16.2.1.1:</p>
                    <p>Download KOReader from the <a href="https://github.com/koreader/koreader/releases" target="_blank">official release page</a></p>
                    <p>Choose the correct package for your Kindle:</p>
                    <ul>
                        <li><code>kindle-legacy</code>: K2, DX, K3 (and all variants)</li>
                        <li><code>kindle</code>: K4, K5, PW1</li>
                        <li><code>kindlepw2</code>: All newer models (PW2, KV, KT2, PW3, KOA, KT3, KOA2, PW4, KT4, KOA3, PW5, KS)</li>
                    </ul>
                </div>
                
                <div class="version-block">
                    <p class="version-label">Firmware >=5.16.3:</p>
                    <p>For newer firmware versions, you need the <code>kindle-hf</code> package</p>
                    <p>Download from <a href="https://fw.notmarek.com/khf/koreader/" target="_blank">Marek's nightly build</a> (recommended)</p>
                    <p class="highlight">As of January 2025, there are no stable releases for Kindle hard float firmware, so you'll need to use a nightly build</p>
                </div>
            </div>
        </div>
        
        <div class="step">
            <h2>Alternative Download Method</h2>
            <div class="stepContent">
                <div class="version-block">
                    <p class="version-label">Firmware <=5.16.2.1.1:</p>
                    <p>No alternative download method needed - use the official release</p>
                </div>
                
                <div class="version-block">
                    <p class="version-label">Firmware >=5.16.3:</p>
                    <p>Alternative options:</p>
                    <ul>
                        <li><a href="https://build.koreader.rocks/download/nightly/" target="_blank">KOReader nightly builds</a> - download the <code>koreader-kindlehf</code> file from the most recent build</li>
                        <li><a href="https://cdn.discordapp.com/attachments/1324761128709914646/1324761128940736675/KoreaderInstall.sh?ex=6783df72&is=67828df2&hm=ba8ae764fe5d387f633333c716fc3bfbcbe3eca75ed2f15d445d8ee9237df61f&" target="_blank">Marek's KOReader downloader scriptlet</a> - Copy this scriptlet into the <code>documents</code> folder on your Kindle, run it from your Library, and it will automatically download and install KOReader</li>
                    </ul>
                    <p class="highlight">Note that these alternative methods might not work for everyone</p>
                </div>
            </div>
        </div>
        
        <div class="step">
            <h2>Connect your Kindle to your computer</h2>
            <div class="stepContent">
                <p>Plug your Kindle into your PC via USB cable</p>
                <p>Wait for your computer to recognize the device</p>
                <p class="highlight">Make sure your Kindle appears as a storage device on your computer</p>
            </div>
        </div>
        
        <div class="step">
            <h2>Install KOReader</h2>
            <div class="stepContent">
                <p>Unzip the downloaded file</p>
                <p>Copy the <code>extensions</code> and <code>koreader</code> folders to the root directory of your Kindle</p>
                <p>When prompted, confirm to merge or replace existing files</p>
                <p class="highlight">If you downloaded Marek's nightly build, you may need to unzip the file twice</p>
            </div>
        </div>
        
        <div class="step">
            <h2>Disconnect and launch</h2>
            <div class="stepContent">
                <p>Safely eject and unplug your Kindle</p>
                <p>Open KUAL (Kindle Unified Application Launcher)</p>
                <p>Look for KOReader in the menu and tap it</p>
                <p>You may see three options:</p>
                <ul>
                    <li><strong>Start KOReader</strong>: Opens KOReader normally</li>
                    <li><strong>Start KOReader (no framework)</strong>: Kills the native GUI first to free up resources and restarts it when you quit</li>
                    <li><strong>Start KOReader (ASAP)</strong>: Skips checks and loads KOReader as fast as possible</li>
                </ul>
            </div>
        </div>
        
        <div class="step">
            <h2>Done</h2>
            <div class="stepContent">
                <p>KOReader is now installed on your Kindle!</p>
                <p>We recommend reading the <a href="https://koreader.rocks/user_guide/" target="_blank">extensive but very helpful guide for KOReader</a></p>
                <p class="highlight warning">Do not connect your Kindle to your PC while KOReader is running, as it may damage files on your device. If you need to charge while using KOReader, use a wall charger or switch to USBNet mode first</p>
                
                <div class="troubleshooting">
                    <h3>Troubleshooting</h3>
                    <p>If KOReader appears in KUAL but doesn't work when clicked:</p>
                    <ol>
                        <li>Delete the <code>koreader</code> folder in the root directory of your Kindle</li>
                        <li>Delete the <code>koreader</code> folder in the <code>extensions</code> directory</li>
                        <li>Download the latest build from <a href="https://fw.notmarek.com/khf/koreader/" target="_blank">Marek's nightly builds</a></li>
                        <li>Reinstall following the steps above</li>
                    </ol>
                </div>
            </div>
        </div>
    </div>
    <div class="buttons">
        <button class="btn btn-orange" id="prev">Previous Step</button>
        <span id="stepCounter"></span>
        <button class="btn btn-green" id="next">Next Step</button>
    </div>
</div>

<style>
.version-block {
    background-color: #1e1e1e;
    border-radius: 8px;
    padding: 12px;
    margin-bottom: 12px;
    width: 100%;
}

.version-label {
    font-weight: bold;
    border-bottom: 1px solid #369d36;
    padding-bottom: 5px;
    margin-bottom: 10px;
    color: #369d36;
}

.troubleshooting {
    background-color: #2a2730;
    border-left: 4px solid #e74c3c;
    padding: 15px;
    border-radius: 0 8px 8px 0;
    margin-top: 20px;
    width: 100%;
}

.troubleshooting h3 {
    margin-top: 0;
    color: #e74c3c;
}

/* Make sure both firmware instructions are clearly visible */
.stepContent {
    align-items: stretch;
}
</style>

<script>new Guide("guide");</script>

## Credits

- Written by Bucks, adapted from the [official KOReader Github installation page](https://github.com/koreader/koreader/wiki/Installation-on-Kindle-devices#err-there-are-four-kindle-packages-to-choose-from-which-do-i-pick)
