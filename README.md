# 14_pre_commit_hook

# How to use pre-commit hook:<br />
1. Move file "pre-commit" under project to 14_pre_commit_hook\\.git\\hooks.<br />
2. Open file and change \<path_to_test\> to real path where tests are situated.<br />
For example:<br />
python D:\\project\\14_pre_commit_hook\\tests.py<br />
3. Save the file.
4. Under project folder run (to get the permissions and only once):<br />
chmod +x .git/hooks/pre-commit<br />
5. Do some changes in any file and in command line run:<br />
git add file_name.py<br />
git commit -m "some changes"<br />
6. If tests pass, changes will be committed. If tests fail, commit will be canceled.