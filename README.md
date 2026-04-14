# IOS xc framework

Select the `lua_public` TARGET and click run to compile. After compilation succeeds, the folder will open automatically.

[Reference article](https://zhuanlan.zhihu.com/p/677506571)


For Android, please refer to [android-lua-lib](https://github.com/aa2013/android-lua-lib)

For macOS, please refer to: [mac-lua-dylib](https://github.com/aa2013/mac-lua-lib)


## CI

This repository includes a GitHub Actions workflow:

- File: `.github/workflows/ios-xcframework-ci.yml`
- Trigger: `push` (`main`/`master`), `pull_request`, `workflow_dispatch`
- Job platform: `macos-latest`
- Output artifact: `LuaFramework-xcframework`

The workflow builds target `lua_public`, validates `Products/LuaFramework.xcframework`, then uploads it as a downloadable artifact.
