# 14_pre_commit_hook

# How to use pre-commit hook:<br />
1. Move file "pre-commit" under project to 14_pre_commit_hook\\.git\\hooks.<br />
2. Open file and change \<path_to_test\> to real path where tests are situated.<br />
For example:<br />
python D:\\project\\14_pre_commit_hook\\tests.py<br />
3. Save the file.
3. Under project folder run (to get the permissions and only once):<br />
chmod +x .git/hooks/pre-commit<br />
4. Do some changes in any file and run:<br />
git add file_name.py<br />
git commit -m "some changes"<br />
5.If tests pass, changes will be committed. If tests fail, commit will be canceled.