# Verify your download

Each release publishes a checksum file, **SHA256SUMS.txt**. If the checksum of the file you downloaded matches the one in that list, the file is the one we published and nothing changed on the way.

## Check the checksum

1. Download **StudioSpend-macOS.dmg** and **SHA256SUMS.txt** from the same [release](https://github.com/lithopoint/studiospend-public/releases/latest).
2. Open **Terminal** and go to your Downloads folder:

   ```bash
   cd ~/Downloads
   ```

3. Compare. This prints `OK` when the file matches:

   ```bash
   shasum -a 256 -c SHA256SUMS.txt --ignore-missing
   ```

   If you see `FAILED`, delete the file and download it again. If it still fails, tell us (see [SUPPORT.md](../SUPPORT.md)) and do not open it.

## Check Apple's signature

After you drag the app to Applications, this confirms it is signed with our Developer ID and that Apple notarized it:

```bash
codesign --verify --deep --strict --verbose=2 /Applications/StudioSpend.app
spctl --assess --type execute --verbose=2 /Applications/StudioSpend.app
```

The second command should end with `accepted` and `source=Notarized Developer ID`. The signing identity is **Developer ID Application: Michael Leonardo (7CCY2MU36M)**.
