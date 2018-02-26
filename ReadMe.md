### 热更新步骤：
1.打基础包：在Terminal中执行命令gradlew assembleDebug 命令，将在build目录下生成一个bakApk文件夹，其中包含基础包

2.修改build.gradle 中的tinkerOldApkPath以及tinkerApplyResourcePath等文件名，然后在Terminal中执行gradlew tinkerPatchDebug 命令，将在build/outputs/apk/tinkerPatch目录下生成一个patch_signed_7zip.apk文件，这个就是差量包

3.将差量包放到TinkerInstaller.onReceiveUpgradePatch(getApplicationContext(), Environment.getExternalStorageDirectory().getAbsolutePath() + "/patch_signed_7zip.apk")对应的目录下

4.点击LOAD PATCH按钮，显示加载成功的吐司然后重启APP即可