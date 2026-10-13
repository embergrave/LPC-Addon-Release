```text
+--------------------------------+
|     L       PPPP      CCCC     |
|     L       P   P    C         |
|     L       PPPP     C         |
|     L       P        C         |
|     LLLLL   P         CCCC     |
+---+   +------------------------+
    |  /
    | /
    |/
```

# LPC Addon

Pre-written character dialogue and emotes for World of Warcraft: Forever.

[Download LPC.zip](https://github.com/embergrave/LPC-Addon-Release/releases/download/current/LPC.zip) · [Verify the download](#verify-the-download)

This repository provides one current readable runtime package. The Release title and provenance identify its version and development status.

## Install and prepare your persona

1. Close World of Warcraft: Forever.
2. Download **LPC.zip**, extract it, and place the complete **LPC** folder under `Interface/AddOns/`. Keep `LPC.toc` directly inside that folder.
3. Start the game, enable LPC, and run `/lpc status` and `/lpc help`.

There is no installer. The catalogue is empty: dialogue requires your own current-format persona, compiled with compatible LPC tooling. Persona JSON alone does not install dialogue, and the compiler is not bundled in this runtime ZIP. Obtain the compatible tools and authoring instructions from the maintainer before preparing a persona.

Use `/lpc personas` to list installed content. Set `/lpc volume 3`, select `/lpc persona <id>` using a listed ID, then run `/lpc enable`. Volume filters dialogue priorities, not sound volume. `/lpc disable` pauses output.

LPC targets Forever's reviewed 1.60.x client family; other WoW products are unsupported. Public output is limited to permitted outdoor contexts. SAY needs fresh eligible player input; EMOTE can use a timer. Client evidence is build-specific; the package does not establish new native game acceptance. Consult its README and Release notes for compatibility limits.

## Update

Close the game and back up the installed addon, authored personas and character data. Install the complete replacement package and recompile your personas: runtime ZIPs contain an empty catalogue. Keep your SavedVariables and check `/lpc status` afterward. Personas use schema 1 / engine 2; pre-1.0 updates support only the current format and may require authoring changes.

## Verify the download

Compare the ZIP's SHA256 with [LPC.zip.sha256](https://github.com/embergrave/LPC-Addon-Release/releases/download/current/LPC.zip.sha256). The stable filename stays **LPC.zip**; [release-provenance.json](https://github.com/embergrave/LPC-Addon-Release/releases/download/current/release-provenance.json) identifies the version and source revision, and `package-files.json` inside the ZIP records file hashes.

GitHub's automatic **Source code (zip/tar.gz)** archives contain documentation and approved documentation assets, not the addon or private development code. Use the named runtime Release asset above.

## License and notices

Original LPC code may be downloaded, inspected and used personally, including personal copies. Redistribution, rehosting or sale, including modified copies, requires permission from the applicable copyright holder. All other rights are reserved. Independently authored persona rights, third-party licenses, existing contributor permissions and nonwaivable rights are unaffected.

The full LPC Source-Available Notice and as-is disclaimer are in the ZIP's `README.md`; third-party notices are in `THIRD-PARTY-NOTICES.md`. These are source-available terms, not an OSI open-source license. No warranty is provided to the extent permitted by law.
