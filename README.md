# GalacticADE IDE - Public-Downloads
GalacticADE IDE public downloads. No source code.

GalacticADE IDE is currently for Windows 11 only since my PC is in storage and my laptop does not have enough storage to operate Linux in Virtual Box.

## To run the app

The executable:
```bat
./GalacticADE.exe
```

To activate telemetry, use the `--TEL` flag, like:
```bat
./GalacticADE.exe --TEL
```
or the long form, `--TELEMETRY`:
```bat
./GalacticADE.exe --TELEMETRY
```

To view the help, use the flag, `--?`:
```bat
./GalacticADE.exe --?
```
or the long form, `--HELP`:
```bat
./GalacticADE.exe --HELP
```

## Telemetry key combinations

With telemetry enabled, you can press the following key combinations to activate various tests:

`Ctrl+Alt+Shift+P` \\ <PageUp> and <PgDown> tests
`Ctrl+Alt+Shift+M` \\ Minimap scrolling tests
`Ctrl+Alt+Shift+T` \\ Quick and simple insertion, undo, and redo test
`Ctrl+T` \\ Insertion of a little over 10 million characters, complete undo (one character at a time), and redo.
`Ctrl+W` \\ Toggle Word-Wrap


## Technical details

- GalacticADE IDE is coded in C++23 and powered by SDL3, the Vulkan graphics API, FreeType font library (to load glyph outlines only), and various others.
- Minimum Vulkan version required: v1.3
- Minimum VRAM: 2 GiB

## Telemetry test results

### Computer:

| Item                                | Value                                                                                           |
| ----------------------------------- | ----------------------------------------------------------------------------------------------- |
| Computer                         | HP Laptop                                                                                    |
| Compiler                            | Clang 23.1.3 |
| Platform                            | Windows 11                                                                                        |
| CPU                                 | Intel64 Family 6 Model 140 Stepping 1, GenuineIntel                                             |
| Logical processors                  | 4                                                                                               |
| Physical RAM                        | 7.65 GiB                                                                                        |
| Selected GPU                        | Intel(R) UHD Graphics                                                                           |
| Vulkan API                          | 1.3.271                                                                                         |
| GPU selection                       | Only compatible Vulkan graphics device detected                                                 |
| Window logical size                 | 1920 × 1009                                                                                     |
| Window pixel size                   | 1920 × 1009                                                                                     |

### Tests:
- Time to load, stylize, and render the first frame of a 1'179 MiB test source code file: 2.235 seconds
- Time to load, stylize, and render the first frame of a 7'324 Mib test source code file: 18-22 seconds

## Some current features:
- Unlimited undo / redo
- Utilizes virtual memory to keep main memory usage down to a minimum
- Files are restored if the app is closed or crashes. Unsaved files remain intact when app is reopened.
- Able to quickly and near-instantly open files and documents in new windows. New windows are created by the GalacticADE IDE instance so memory is not copied or moved between them, causing the switching between the main app to a new window to be near instant.
- Provides a document, directory, and project panel that displays those that are currently open.
- GalacticADE IDe is faster and more responsive than Microsoft's Visual Studio Code and Sublime Text.
- Microsoft's Visual Studio code can not open files over 1 GiB due to the JavaScript engine it uses.
- GalacticADE IDE opens and stylizes faster than Microsoft Visual Studio Code and Sublime Text. While GalacticADE can open a 7.5 GiB textual file in 18-22 seconds, Sublime Text was manually closed after 5 minutes of waiting to open the same document.
- GalacticADE IDE offers an easy to create theming system.

## Final Notes

- GalacticADE IDE is in the Alpha stage and normally should not be available for public testing. The decision was made to provide these versions for those who wish to help test the product at its earliest stages. Due to the current stage the project is at, there will be features and systems that are not implemented that are found in other IDEs and editors.
- If you have any suggestions, comments, issues, find bugs, or anything else that you would like to mention about, please create an issue.
- When the Discord server is implemented, discussions and chats can be done there.

