# ��������GitHub �ɓo�^���܂��傤�C�ȉ����̑O��ŁD

## GitHub �T�C�g��ŁC���|�W�g���������URL���擾���Ă����D

## local �̃f�B���N�g�������|�W�g���� push ����D
https://qiita.com/bakainubau/items/4613dda50a5fa302d212
1. ���̃f�B���N�g���Ɉړ����C`git init`
2. `git add .` `git commit -m "FirstCommit"`
3. `git remote add origin https://github.com/Okdenn/HowtoGitHub.git`, URL�͓K�X���|�W�g�����Ƃɕς���D
4. `git push origin master` �Ŋ����D��͕��i�ʂ�C�t�@�C����ҏW���C`git add hogehoge`, `git commit -m "hogepiyo"`, `git push origin master`���邾���D
### ���܂ɃT�C�g�Ń��|�W�g�������O�� local repository �� commit ���Ă��܂����Ƃ�����i�Ȃ�����j�D���̍ۂ́C���1-3�܂ł͓����ŁChttps://qiita.com/takanatsu/items/fc89de9bd11148da1438
5. `git fetch`
6. `git merge --allow-unrelated-histories origin/master` �Ƃ��Ĕ������I�Ƀ}�[�W����D���̌� `git push origin master` �Ŋ����D
