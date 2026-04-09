# IOS xc framework

Select the `lua_public` TARGET and click run to compile. After compilation succeeds, the folder will open automatically.

[Reference article](https://zhuanlan.zhihu.com/p/677506571)

## CI

This repository includes a GitHub Actions workflow:

- File: `.github/workflows/ios-xcframework-ci.yml`
- Trigger: `push` (`main`/`master`), `pull_request`, `workflow_dispatch`
- Job platform: `macos-latest`
- Output artifact: `LuaFramework-xcframework`

The workflow builds target `lua_public`, validates `Products/LuaFramework.xcframework`, then uploads it as a downloadable artifact.
