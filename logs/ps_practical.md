# ps practical

i opened  the repo and started my log. 

## cheese commit: 
bad commit: **2ded3c2...** (msg: "do something again")

issues i saw:
- `FileCheeseStream` instead of `FileOutputStream`
- `scanner.cheese()` not `scanner.nextLine()`
- `} cheese (` should be `} catch (`
- var named `cheese` where it shd be `passwordBytes`

basically cheese nuked parts of `ReversibleEncryptor.java`.

## finding the passwrd
pingd the pi (~5s). it answers fine.
ssh’d into `pi@192.168.1.187` (pwd: raspberry). did a quick find on dotfiles/secret stuff.
found a dir: `.git-practical-secret-directory` with file saying:

password = `24732473`.

## decrypt plan (but code broke)
`ReversibleEncryptor.java` reads `.env` for the key, then XORs.
`24732473` is in `.env` (gitignored so it won’t show in changes). but the java file still has cheese typos, so won’t compile and run.

why only log changed?
- `.env` is in `.gitignore` -> not tracked
- i only read the java file, didn’t fix it here
- so only `logs/ps_practical.md` shows edits

todo next (if we wanna run it):
- revert the cheese commit or fix the typos
- `javac ReversibleEncryptor.java`
- run with `encrypted.txt` and write to `decrypted.txt`

