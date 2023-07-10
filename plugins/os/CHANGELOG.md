# Changelog

## \[2.0.0-alpha.1]

- [`1091d6d`](https://github.com/tauri-apps/plugins-workspace/commit/1091d6d6ac5081f2c7526b0f492ae4f34b306f1d)([#419](https://github.com/tauri-apps/plugins-workspace/pull/419)) The os plugin is recieving a few changes to improve consistency and add new features:

  - Renamed `Kind` enum to `OsType` and `kind()` function to `os_type()`.
  - Added `family()`,`exe_extension()`, and `hostname()` functions and their equivalents for JS.
  - Removed `tempdir()` function and its equivalent on JS, use `std::env::temp_dir` instead of `temp_dir` from `tauri::path::PathResolver::temp_dir` and `path.tempDir` on JS.
  - Modified `platform()` implementation to return `windows` instead of `win32` and `macos` instead of `darwin` to align with Rust's `std::env::consts::OS`
  - `EOL` const in JS has been modified into a function `eol()` fix import issues in frameworks like `next.js`

## \[2.0.0-alpha.0]

- [`717ae67`](https://github.com/tauri-apps/plugins-workspace/commit/717ae670978feb4492fac1f295998b93f2b9347f)([#371](https://github.com/tauri-apps/plugins-workspace/pull/371)) First v2 alpha release!
