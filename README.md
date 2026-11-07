# llvm-artifacts

binaries created by [llvm-wasm](https://github.com/Ambeco/llvm-project), consumed by [vscwClang](https://github.com/Ambeco/vscwClang).
They're in this separate repo merely so vscwClang's git tree doesn't explode if/when we update the massive binaries, and so we can fetch them remotely from the plugin.


Only `mtdist/` (the multithreaded toolchain layout) is published; the extension pins one tag and loads `mtdist/manifest.json` from it. The single-threaded `dist/` layout was removed after `v24.0.11`; older tags still contain it.
