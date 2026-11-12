# infinity_android_packages_apps_Updater-lineage_hide

将系统更新器（Updater）读取的版本属性从易被检测的 `ro.modversion` 迁移为 `ro.infinity.build.version`。

## 拉取部分代码（Cherry-Pick）

进入目标 ROM 源码的 `packages/apps/Updater` 目录执行：

```bash
cd packages/apps/Updater
git fetch [https://github.com/yokeshiq/infinity_android_packages_apps_Updater-lineage_hide.git](https://github.com/yokeshiq/infinity_android_packages_apps_Updater-lineage_hide.git) main
git cherry-pick cd3c58f
```

## 修改文件清单

- `app/src/main/java/com/infinity/updater/misc/Constants.java`
