### �ȸ��²��裺
1.�����������Terminal��ִ������gradlew assembleDebug �������buildĿ¼������һ��bakApk�ļ��У����а���������

2.�޸�build.gradle �е�tinkerOldApkPath�Լ�tinkerApplyResourcePath���ļ�����Ȼ����Terminal��ִ��gradlew tinkerPatchDebug �������build/outputs/apk/tinkerPatchĿ¼������һ��patch_signed_7zip.apk�ļ���������ǲ�����

3.���������ŵ�TinkerInstaller.onReceiveUpgradePatch(getApplicationContext(), Environment.getExternalStorageDirectory().getAbsolutePath() + "/patch_signed_7zip.apk")��Ӧ��Ŀ¼��

4.���LOAD PATCH��ť����ʾ���سɹ�����˾Ȼ������APP����