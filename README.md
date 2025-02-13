```bash
cd lib

pnpm pack --pack-destination tmp

cd ../app

pnpm i ../lib/tmp/lib-1.0.0.tgz
```

The error is:
```
pnpm: ENOENT: no such file or directory, open 'C:\Users\pmh\AppData\Local\pnpm\store\v10\index\2c\fcca2b5b110b7e66a848cd29e6c490730cfdf7f69df04c05eff0d98f5aae16-lib@1.0.0.json'
```

I found this file in the directory (.../pnpm/store/v10/index/2c/):
  `fcca2b5b110b7e66a848cd29e6c490730cfdf7f69df04c05eff0d98f5aae16-file+..+lib+tmp+lib-1.0.0.tgz.json`

Instead of:
  `fcca2b5b110b7e66a848cd29e6c490730cfdf7f69df04c05eff0d98f5aae16-lib@1.0.0.json`






