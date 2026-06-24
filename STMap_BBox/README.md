# STMap_BBox v1.0.0

## Supported platforms

| OS | Architecture | Nuke versions |
|----|--------------|---------------|
| macOS | arm64 (Apple Silicon) | 14.1, 15.0, 15.1, 15.2, 16.0, 16.1, 17.0 |
| Linux | x86_64 | 15.0, 15.1, 15.2, 16.0, 16.1, 17.0 |

Windows is not included in this release.

If your Nuke major.minor version has no matching binary, the plugin prints a warning at startup and does not load.

## Install

1. Copy the `STMap_BBox` folder into your Nuke plugin path.  For example:

   Move or copy into your `~/.nuke/` folder

2. **Mac users only: run one command in Terminal**

   When you download files from the internet on a Mac, the system may block Nuke from opening the plugin. This is normal. The plugin is not broken.

   If you skip this step, Nuke may show a long error that includes: `library load disallowed by system policy`

   **How to fix it (do this once after you copy the folder):**

   1. Open **Terminal**.
   2. Copy the line below, paste it into Terminal, and press **Enter**:

      ```bash
      xattr -cr ~/.nuke/STMap_BBox
      ```

   3. If you put the `STMap_BBox` folder somewhere other than `~/.nuke/`, change the path in that line to match your folder.

   **Linux users:** skip this step.

3. Add this line to `~/.nuke/init.py` (create the file if missing):

   ```python
   nuke.pluginAddPath("./STMap_BBox")
   ```

   Alternatively, point to wherever on the server you placed the `STMap_BBox` folder:

   ```python
   nuke.pluginAddPath("/Replace/With/Path/To/Your/STMap_BBox")
   ```

4. Restart Nuke. Find the node under **Nodes → Transform → STMap_BBox**, or type `STMap_BBox` in the Tab search.
